# Trivy — skaner podatności

---

## Co to jest?

**Trivy** (od Aqua Security) to wszechstronny, open-source'owy skaner bezpieczeństwa. Skanuje:
- **Obrazy kontenerów** (Docker, OCI)
- **Systemy plików i repozytoria** (kod źródłowy)
- **Infrastrukturę jako kod** (Terraform, CloudFormation, Kubernetes YAML)
- **SBOM** (Software Bill of Materials)
- **Klastry Kubernetes** (w locie)

GitHub: github.com/aquasecurity/trivy

---

## Co wykrywa?

| Typ | Opis |
|-----|------|
| **Podatności (CVE)** | Znane podatności w pakietach OS i bibliotekach aplikacji |
| **Misconfigurations** | Błędy konfiguracji w IaC (Terraform, Docker, K8s) |
| **Secrets** | Wycieki haseł, kluczy API, tokenów w kodzie |
| **Licenses** | Analiza licencji zależności |

---

## Instalacja

```bash
# macOS
brew install trivy

# Linux (Debian/Ubuntu)
sudo apt-get install trivy

# Docker
docker run aquasec/trivy image python:3.9
```

---

## Najczęstsze użycie

### Skanowanie obrazu Docker
```bash
trivy image nginx:latest
trivy image --severity HIGH,CRITICAL myapp:v1.2
```

### Skanowanie projektu (filesystem)
```bash
trivy fs .
trivy fs --scanners vuln,secret,misconfig .
```

### Skanowanie repozytorium Git
```bash
trivy repo https://github.com/user/project
```

### Skanowanie IaC (Terraform, K8s YAML)
```bash
trivy config ./terraform/
trivy config ./k8s-manifests/
```

### Skanowanie klastra Kubernetes
```bash
trivy k8s --report summary cluster
```

---

## Filtrowanie wyników

```bash
# Tylko HIGH i CRITICAL
trivy image --severity HIGH,CRITICAL nginx:latest

# Ignoruj podatności bez poprawki
trivy image --ignore-unfixed nginx:latest

# Wyjście jako JSON
trivy image -f json -o results.json nginx:latest

# Wyjście jako tabela z CVSS score
trivy image --format table nginx:latest
```

---

## Integracja z CI/CD

### GitHub Actions
```yaml
- name: Run Trivy vulnerability scanner
  uses: aquasecurity/trivy-action@master
  with:
    image-ref: 'myapp:${{ github.sha }}'
    format: 'sarif'
    output: 'trivy-results.sarif'
    severity: 'HIGH,CRITICAL'
```

### GitLab CI
```yaml
trivy-scan:
  image: aquasec/trivy:latest
  script:
    - trivy image --exit-code 1 --severity HIGH,CRITICAL myapp:latest
```

---

## Trivy vs inne skanery

| Cecha | Trivy | Grype | Snyk | Clair |
|-------|-------|-------|------|-------|
| Open source | ✅ | ✅ | Freemium | ✅ |
| Kontenery | ✅ | ✅ | ✅ | ✅ |
| Filesystem/kod | ✅ | ✅ | ✅ | ❌ |
| IaC scanning | ✅ | ❌ | ✅ | ❌ |
| Secrets | ✅ | ❌ | ❌ | ❌ |
| K8s cluster | ✅ | ❌ | ✅ | ❌ |
| Szybkość | Szybki | Szybki | Średni | Wolny |

---

> **Moje przemyślenia:**
> *(tu wpisuj swoje notatki)*
