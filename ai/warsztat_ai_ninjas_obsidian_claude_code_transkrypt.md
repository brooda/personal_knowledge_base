# Warsztat AI Ninjas — Zbuduj bazę wiedzy, z której AI sam sięga po kontekst | Obsidian + Claude Code

- **Źródło:** https://www.youtube.com/watch?v=Z0DA634O9w4
- **Prowadzący:** Krzysztof Tutak, Krzysztof Bohaczyk
- **Typ:** transkrypt automatyczny (YouTube auto-captions)

---

Dzień dobry. Dzień dobry moi drodzy.
Witam was serdecznie na kolejnym
warsztacie A Ninjas, który standardowo
prowadzą dla was Krzysztof Tutak i
Krzysztof Bohaczyk.
>> I Krzysztof Bohaczyk. Witam. Witam
również.
>> Standardowo zanim
>> standardowo zanim wskoczymy do
dzisiejszego
tematu, to pytanko do was. Czy nas
widać, słychać i czuć? że będziemy tutaj
wdzięczni, bo y demowie,
bogowie demo zazwyczaj nie są łaskawi.
>> Mam nadzieję, że dzisiaj właśnie będą
wyjątkowo.
>> Mamy już tutaj jednego ninja, który
który ma bardzo dobry węch. To bardzo
dobrze świadczy.
>> Mnie gorzej słychać. Może się spróbuję
przepiąć na drugi mikrofon, to może
będzie lepiej. Ale
>> okej, widać i słychać. Super, wielkie
dzięki. Także tutaj pomału już osoby się
zbierają. Mamy już na pokładzie 120
osób, więc bardzo fajnie, cieszymy się.
Zanim jeszcze wskoczymy do dzisiejszego
tematu, to takie pytanko do ciebie
Krzychu. Co tam ciekawego się wydarzyło
przez ostatni miesiąc?
>> Powiem ci, że dosyć intensywnie. W ogóle
nie mieliśmy nawet okazji się gdzieś tam
zgrać w tym miesiącu. Na pewno było
ciężko. E, dopiero co święta, teraz po
świętach majówka się zaraz szykuje,
także strasznie tych dni ucieka.
Natomiast y pozytywnie, raczej
pozytywnie nie narzekam. Wszystko w
porządku. Dzisiaj nowy warsztat, inny
temat niż zwykle, także też jestem
ciekawy jak to nam wyjdzie i czy wam
temat w ogóle się spodoba. Także to tyle
ode mnie. Może ty Krzyśku tutaj też coś
powiesz, jak ty to w ogóle widzisz.
>> Dla mnie dla mnie to też mega był y
intensywny czas. M ostatni miesiąc.
Sporo rzeczy się tutaj dzieje, zarówno w
kontekście biznesowym, czy też e właśnie
tematów, z którymi działam na co dzień.
Natomiast tutaj już chyba nie ma zbytnio
co przedłużać, więc lecimy tutaj dalej z
tematem. Jak już pewnie tutaj
zobaczyliście teraz na ekranie,
dzisiejszy temat to zbuduj swój second
brain z wykorzystaniem cloud codea i
obsidiana.
I to co będziemy chcieli wam dzisiaj.
Dobra, ale zanim jeszcze tutaj wskoczymy
do tego tematu to może kilka słów o nas.
Krzyśku, może byś rozpoczął?
Tak. No to ja jak jestem tak samo jak
Krzysiek Ninjo, jednym z AI Ninjas,
natomiast na co dzień zajmuję się,
jestem programistą w sektorze
finansowym, gdzie po prostu działam od
strony Full stacku, ale też różnej
integracji z AI. Na co dzień też działam
mocno w social mediach, szczególnie na
LinkedInie i też właśnie teraz na
YouTubie w ramach właśnie edukowania z
wykorzystania po prostu mądrego AI.
I dodatkowo no właśnie prowadzę warsztat
tutaj jako jeden połówka, że tak powiem,
niny, AI ninjas wraz z Krzyśkiem, gdzie
również dzielimy się wiedzą na takich
bezpłatnych warsztatach oraz w naszej
społeczności.
Jeśli chodzi o mnie, to m pewnie część
osób kojarzy mnie z takich inicjatyw jak
podcast bliskie spotkania z AI, który
mam przyjemność prowadzić, czy też może
z konferencji A Miners, którą
organizuję.
Na co dzień zajmuję się
AI już od dłuższego czasu, a ponad 10
lat mam doświadczenia jako programista,
więc tutaj w takim bardzo technicznych
obszarach się poruszałem przez dłuższy
czas.
No i myślę, że tyle. Nie ma co tutaj już
tak zbytnio przedłużać. I jaki mamy plan
jazdy na dzisiaj? Yyy, zaczniemy sobie
od wyjaśnienia koncepcji Second Braina.
Czym w ogóle to jest? Hmm, po co w ogóle
taki budować Second Brain, a następnie
wskoczymy do serii A4 Live Demo, gdzie
pokażemy w jaki sposób można dokonać tej
migracji notatek z Notion Obsidiana.
Pokażemy jak można realizować sobie
research i syntezę wiedzy z
wykorzystaniem właśnie tutaj cloud coda.
a następnie wskoczymy do demo, w którym
poopowiadamy o takim koncepcji, który
ukułowiek
zwany Carpatim, gdzie
pokazuje taki sprytny sposób w jakiej
można stworzyć takie sobie elm wiki, a
następnie skoczymy do kolejnych takich
przykładów, gdzie pokażemy jak można
ocerować dokumenty i wrzucać je
bezpośrednio do naszego obsydianowego
Volta, czy też kilka innych takich casów
pokazujących w jaki sposób można
planować zadania i kilka innych z
wykorzystaniem tutaj właśnie
tego tandemu, czyli cloud code i second
brain. A na sam koniec przejdziemy sobie
do sekcji Q&A. No i oczywiście na koniec
tej części merytorycznej mamy też dla
was jeszcze pewną niespodziankę, którą
będziemy zdradzać później.
>> Dokładnie. Może nie wszystko na starcie.
Dokładnie. Także tutaj już możemy
przejść do tej części
z demo. Przepraszam, nie z demo, tylko
tutaj do wyjaśnienia, czym jest w ogóle
ten second brain. Więc tutaj już oddaję
Majka
Krzyśkowi.
>> Dziękuję bardzo. Ja się tu jeszcze
włączę na pełen ekran. No właśnie, czym
jest w ogóle second brain? Czym jest
budzowanie takiej bazy wiedzy?
I tak krótko zaczynając tutaj tym
slajdem, twoja wiedza zasługuje na
więcej niż tylko wyszukiwarkę. I
mianowicie co mam na myśli?
Ze jest pewien problem
i taki, którego już jak zauważysz to
raczej nie odzobaczysz. I ten problem
nie dotyczy tego, że ja je halucynuję
albo że jest drogie. To z tym musimy się
liczyć na co dzień. Natomiast chodzi o
coś głębszego,
o to jak układamy sobie z nim relacje i
budujemy wiedzę. No bo takie klasyczne
podejście to jest przeważnie większość
po prostu z nas używa jaj w sposób
pytasz, dostajesz jakąś odpowiedź, no i
następnie zamykasz czy to czat, czy to
jakiegoś asystenta. Jutro masz podobne
pytanie, może z tego samego obszaru,
tego samego projektu. No i znowu musisz
zadać pytanie, wytłumaczyć kontekst,
wytłumaczyć w ogóle jajowi z czym mamy
do czynienia. No i na poziomie
pojedynczego pytania to jest całkiem
dobre, ale zatrzymajmy się i spójrzmy,
co tu się właściwie dzieje. Każde
pytanie startuje od zera, tak? Czyli AI
nie pamięta co wczoraj tak naprawdę
dostał od ciebie. Nie pamięta też, że
zadawałeś podobne pytania tydzień temu
czy miesiąc temu. Nie pamięta w jakim
miejscu jest twój projekt. Nie zna
kontekstu tak naprawdę tego, co się
dzieje wokół ciebie na co dzień i nic
się nie zapisuje. Tak przynajmniej tak
patrząc na takich asystentów
przeglądarkowych. Mamy oczywiście tam tą
sekcję memory, ale tak patrząc na
takiego podstawowego asystenta, no to
ten kontekst faktycznie się nie składa.
Praca, którą włożyłeś dzisiaj na
sformułowanie dobrego prompta,
wytłumaczenia czegoś asystentowi, jutro
wyparuje. No i mamy taki mechanizm. Ten
mechanizm ma pewną nazwę RAC, czyli
Retrieval Augumented Generation. To jest
technika, której używa chociażby chat
GPT, jak wrzucisz mu pliki, notebook LM,
clot z załącznikami. Wszystko to działa
w tym samym schemacie, czyli wrzucasz
dokumenty, AI je indeksuje do do
wektorów, zadajesz pytanie, AI wyciąga
pasujące fragmenty, czyli te czanki, a
następnie składa z nich odpowiedź, tak?
Czyli jest w stanie na bazie twoich
jakichś dokumentów, załączników
faktycznie przetwarzać i wyciągać
informacje. Działa to jak najbardziej w
tych asystentach przeglądarkowych, ale
każde kolejne pytanie, no rak zaczyna po
prostu od zera, szuka, wyciąga, składa i
tak dalej od początku. I to co właśnie
wcześniej mówiłem, nic się składa, to
znaczy to jest jeden z tych problemów,
czyli nic nie rośnie w czasie. Czyli
wyobraź sobie takiego badacza, który
powiedzmy tygodniami czyta różne
publikacje naukowe i teraz gdybyś mu
powiedział: "Hej, jutro zapomnisz
wszystko". No to to brzmi dosyć
absurdalnie, ale tak to właśnie działa
czyli to co dokładnie robimy z AI na co
dzień. Z czasem zauważysz, że po prostu
pracujesz dla AI. Musisz za każdym razem
tłumaczyć mu kontekst po raz piąty, 10 w
tym samym miesiącu, zamiast po prostu
zrobić, żeby AI pracowało dla ciebie i
było świadome tych projektów i narzędzi,
z którymi działasz na co dzień. I to co
ostatnio taka publikacja, którą
przygotował Karpati, czyli
współzałożyciel Open AI, były szef AI
Tesli, to przygotował taki, można
powiedzieć dokument, gdzie wytłumaczył
jak może działać. taka personalna baza
wiedzy Wiki, on to tak nazywa. Yyy i
wrzucił właśnie na Twittera post i
dołożył takiego właśnie dłuższego Gista,
taki plik właśnie dokumentowy. Jednym
zdaniem przewrócił ten model do góry
nogami. Może troszeczkę tutaj
podkoloryzowuję, bo to może nie jest coś
nowego, natomiast można powiedzieć, że
dał temu tematowi drugie życie.
Czyli Obsydian to ID, LM to programista
i wiki to codebase. Obsydian jako
narzędzie właśnie do zarządzania tym
naszym tą naszą bazą wiedzy. LM, czyli
nasz model, tworzy właśnie te różne
powiązania, a wiki to jest to nasze
źródło, które ta cała właśnie wiki,
którą utrzymujemy, tak? To jest kod,
tak? kod czy właśnie różna struktura
plików i chciałbym, żebyś na chwilę
tutaj z nami uczestniku tego liveu
zatrzymał się nad tym zdaniem. Jak to
rozpakujesz to po prostu zmienia to
pewien sposób myślenia o notatkach. AI
już nie wyszukuje. Nie tyle wyszukuje,
ale też buduje. I tu jest pewny switch,
który trzeba zauważyć. Czyli zamiast
zadawać pytanie i kazać szukać po
dokumentach, dajesz mu rolę takiego
programisty, badacza, który utrzymuje
twoje twoje repozytorium, twoją bazę
wiedzy. Tyle, że ten ten code base,
twoje repozytory to nie jest sam kod,
tylko właśnie tak jak mówię różne
notatki, różna syntetyzowana wiedza,
podsumowania i teraz one są zlinkowane
między sobą, czyli mogą do siebie
również te różne notatki nawiązywać. Tak
więc to jest też bardzo ważne, czyli
rosną również w czasie po prostu jak
rozwija się to repozytorium, rozwija się
twoja baza wiedzy, to one też po prostu
rosną wraz z tobą. AI czyta nowe źródła
i aktualizuje istniejące strony. Tworzy
nowe tam, gdzie po prostu jest to
wymagane. Więc synteza robi się raz, a
potem rośnie. Czym jest w ogóle Volt?
Jest takie, jest takie określenie w w
terminologii Obsydiana. Volt to jest nic
innego jak folder, czyli to co też jest
dużą przewagą tego narzędzia Obsidian, o
którym dzisiaj będziemy tutaj
rozprawiać, to to, że tak naprawdę pod
spodem to jest zwykły folder na waszym
pulpicie czy w jakimkolwiek innym
katalogu, który zawiera pliki Markdown i
to jest na tyle proste. Także pierwsza
też rzecz albo dodatkowa, którą tutaj
daje nam przewagę obsydian, to to, że
nie mamy vendor logina, czyli prosto
mówiąc nie jesteśmy związani z żadnym
dostawcą. Równie dobrze możemy
odinstalować tego naszego obsydiana i
dalej z nim działać w ramach tych po
prostu plików, tej płaskiej struktury,
którą wypracowaliśmy.
No dobrze. I pod spodem to, co
powiedziałem przed chwilką, to są różne
pliki Markdown, które mogą znajdować się
na twoim dysku. I teraz jak jutro
chociażby Obsydian wniknie, no to dalej
te notatki zostają u ciebie na
komputerze, także nie musisz w ich żaden
sposób na nowo pobierać. Yyy, także to
co ja gdzieś tam moje takie przemyślenia
na ten temat, czemu w ogóle obsydian i
czemu zacząłem też korzystać z
obsydiana, a mianowicie przez trzy lata
prowadziłem Notion, rozwijałem swoją
bazę wiedzy, taki second brain z
notatkami przez y przez no właśnie długi
okres, trzy lata. I na moim przykładzie
dużo z tych notatek, czy to właśnie
projekty, research, jakieś różne wyciągi
z książek, no tej wiedzy było bardzo
dużo. Natomiast w pewnym momencie im
więcej tych tych rzeczy miałem, tym
rzadziej do tego zaglądałem. A to z tego
powodu, że oprócz dodawania nowych
rzeczy, to trzeba się też zajmować
utrzymaniem takiego naszego seconda. No
i moje notatki często stawały się już
cmentarzyskiem. Często do niektórych z
notatek w ogóle nie byłem w stanie
wrócić, nie byłem w stanie się połapać w
strukturze, gdzie one właściwie są, więc
było na pewno ciężko. No i właśnie tutaj
to są też powody, dlaczego mój no umarł,
czyli no nie było czegoś takiego jak
integracja z AI, nie mógł mi AI
przeglądać, wyciągać tych danych. Jeśli
chodzi o MCP, no bo dzisiaj mamy coś
takiego w Notion jak MCP, czyli jesteśmy
w stanie ułączyć się naszymi agentami do
tego, do tej bazy wiedzy i wyciągać
informacje. To samo MCP jest dosyć
toporne, zżera dużo tokenów, to
wyszukiwanie działa słabo i dosyć
punktowo i często gubił po prostu jakieś
treści, których szukałem albo no były
problemy, musiałem wiele razy iterować,
żeby dostać konkretny dokument, a już
nie mówię o edycji. No i też Notion
wymagał takego remontu, o którym
powiedziałem. Jeśli miałbym to robić
ręcznie, no to zajęłoby mi na pewno to
parę tygodni.
Także to, co ja zrobiłem nawet przed tym
jeszcze jak przygotowaliśmy się jeszcze
przed tym warsztatem, to pierwsza rzecz,
która mi przyszła na myśl, czemu nie
wyeksportować tego właśnie do obsydiana
i zarządzać tym lokalnie. Obsydian
świetnie pracuje teraz chociażby po
różnych y CLI, czyli rozwiązaniach,
takich narzędziach terminalowych z
właśnie asystentami, z agentami. I tutaj
eksport takiego pliku zajął mi mojego
wielkiego notion zajął mi niecałą
godzinkę. To akuratnie po API było
wszystko wyciągane. Później Clot zrobił
audyt, stwierdził co jest do poprawy,
jakie linki są już przestarzałe,
nieaktualne i też był w stanie otagować
je i przygotować mi taką bazę wiedzy. I
to też chcę wam dzisiaj pokazać. Także
już tak słowem wstępu yy trochę się
rozgadałem, natomiast przejdźmy i pokażę
wam w praktyce jak wy możecie to zrobić
u siebie.
Oczywiście jeśli chodzi o obsydian, to
co pokażę jeszcze, to nie musimy
oczywiście zamykać się tylko do tylko do
konkretnie notion. Oczywiście te
integracje działają z wieloma innymi
narzędziami. Tutaj z takich rzeczy,
którym możemy się integrować to
chociażby Notion. Natomiast mamy też
Evernotea, mamy też chociażby Google
Notes, na przykład notatki w iOSie,
także jest tego bardzo, bardzo dużo i
nie musimy za to płacić, bo to narzędzie
jest w pełni darmowe, także to też jest
ważny punkt. I teraz jak możemy w ogóle
sobie takie integracje zrobić? Ja tu
jeszcze tylko na szybko chcę pokazać
właśnie to, co będziemy dzisiaj
pokazywać. Są pewne pluginy stworzone
przez społeczność. I z tego powodu, że
to jest rozwiązanie dostępne za darmo,
no to jest duża społeczność za tym
projektem i ludzie dzielą się różnymi
przemyśleniami i też różnymi pluginami,
rozwiązaniami do swoich obsydianów. I
takim jednym z najpopularniejszych
wtyczek to jest właśnie importer. On
właśnie nam ułatwia tą całą integrację.
Zobaczcie, tutaj są przeróżne przeróżne
narzędzia jakby bear, mamy everne,
notion, one apple notes. Także można się
tutaj z tym zaznajomić. Można nawet
zwykłe pliki Markdown, ZLCEN. Mamy też
zwykłe pliki HTML, także jest tego dużo,
dużo. Wy możecie oczywiście na czacie
napisać, gdzie wy macie na przykład
swoje notatki, gdzie wy je
przetrzymujecie, więc to też można
później w ramach Q&A poruszyć ten temat,
jak można to sprytnie zaimportować. Ja
dzisiaj na tapet wziąłem Notion i tutaj
mamy parę sposobów. albo przez API,
czyli będziemy musieli wygenerować sobie
integrację po stronie Notion,
wygenerować swój klucz i następnie
będziemy mogli
za pomocą tego klucza po prostu sobie te
notatki ściągnąć. Mamy też file import,
czyli po prostu wchodzimy na nasz notion
do general zakładki ogólne i możemy
wyeksportować pliki. Tutaj jeśli chodzi
o ten eksport, on nie jest aż taki dobry
jak po API. Często te informacje są
gubione. Dostawałem bardzo dużo błędów
przy takim przy takim porcie. Także
tutaj jeśli macie opcję zrobienia tego
po API to trwa o wiele dłużej, natomiast
jakość tego codebaseu jest o wiele
lepsza. I też jest coś takiego jak
noteion zip, czyli możemy po prostu
pobrać całego zipa i też go sobie
zaimportować. Ja akuratnie też przy tym
y przy tym konkretnym imporcie miałem
problemy, ale przejdźmy teraz na
szybciutko do notion, to może wam pokażę
jak to u mnie w praktyce wygląda. W
ogóle zacznijmy od notion, żeby było,
żeby nie było, że ja to wymyśliłem i i
że to nie jest właśnie moje notion.
Także tutaj oczywiście bez pokazywania
jakieś bardzo szerokiej listy tych
notatek, które mam w tym Notion, no to
mamy jakieś różne page. To jest właśnie
moja baza wiedzy, która sobie tutaj
buduję przez lata. I teraz jest coś
takiego jak settings. Jak przyjdziemy do
ustawień, to będziemy mogli sobie
chwileczkę. to będzie tutaj settings, to
będziemy mogli sobie taką integrację
tutaj w connections wygenerować. Mam tu
już różne aplikacje podpięte, natomiast
co będziemy musieli zrobić to stworzyć
sobie właśnie taki nowy connection. I
teraz ja już mam tutaj tego obsydiana
połączonego. On może sobie po tym appi
korzystać. Stąd mogę sobie skopiować mój
integration token. I teraz jak mam
skopiowany ten token, to mogę wrócić do
naszego obsydiana. Yyy, jeśli chodzi o
instalację obsydiana, jest to bardzo
proste, bo wystarczy wpisać Obsydian
download i linki też są na internecie.
Oczywiście podrzucimy to w ramach takiej
notatki podsumowującej po warsztacie na
wasze maile. I teraz to, co widzicie po
lewej stronie, to są przeróżne
struktury, które ja tutaj mam w ramach
mojego yyy Notion. I jak ja to w ogóle
zaimportowałem wszystko. No bo nie
robiłbym tego oczywiście ręcznie, bo to
by mi zajęło bardzo, bardzo długo. Ale
to co powiedziałem wcześniej, mamy
wtyczki. I teraz jak przejdziemy sobie
do przeglądania wtyczek, tutaj widzę, że
aktualnie mam jakiś problem, ale pokażę
wam może drugie też repozytorium, drugi
notion, który mam tutaj na boku też
odpalony, który w którym budowałem sobie
tak naprawdę też notatki w ramach
obsydiana, czyli zrobiłem sobie osobnego
Volta, w którym badam co można
potencjalnie zrobić ciekawego jeszcze z
obsydianem. To jest takie źródło dla
mnie wiedzy, w którym rozbudowuję sobie
właśnie w tym konkretnym temacie. I
jeśli wejdę tutaj w te wtyczki
preferences,
proszę bardzo, wbudowane wtyczki. Ja już
mam ich troszeczkę poinstalowanych i też
postaram się je omówić później, jak
jeszcze po Krzyśku prezentacji, jak
będziemy mieć chwilę, ale takie
najważniejsze, co ja mam, to właśnie
importer. Nie wiem czemu akuratnie
dzisiaj jest jakiś problem. To tak jak
zwykle przy demo. Generalnie jeśli mamy
zainstalowanego tego importera to jak y
tutaj z poziomu wtyczek społeczności jak
dodamy sobie tego importera, możemy go
śmiało wyszukać w importer. Dzisiaj
widzę, że jest jakiś problem. Wyświetli
wam się tutaj jako plugin i następnie
jak go zainstalujemy, klikamy
zainstaluj. To jest bardzo intuicyjne.
Tutaj ptaszkiem z poziomu wtyczki
społeczności będziemy musieli go
włączyć, to on nam się pojawi tutaj po
lewej stronie w zakładkach. Ja może to
zzoomuję, bo wiem, że ekran może być
malutki. O, proszę bardzo, będzie
lepiej. Mamy open importer. I co tu
ciekawego? Mamy różne file formaty,
czyli możemy importować CSV, Google
Keep, Everne, to co mówiłem wcześniej.
Więc my wybieramy Notion i tutaj
wprowadzamy swój token. Następnie mamy
załadowane też tabelki, które które
wskazują nam, o, ja może widzę, że teraz
teraz akurat nie tego tokena nie
skopiuję. Natomiast jak już pobiorę ten
koken, to tu będę mógł sobie zobaczyć
jakie konkretne tabele mam do
załadowania. możemy wybrać, oczywiście
nie musimy wybierać wszystkich. Możemy
też dodać tutaj import, taki
inkrementalny, czyli jak w przyszłości
będziemy importować jakieś rzeczy z
Notion, to nie będzie na nowo dodawać
tych samych Pagey, ale sprawdzi, które
są nowe i zaimportuje te, które są no
właśnie zaktualizowane lub jakieś
nowsze. I tutaj są różne ustawienia
jeszcze do tego, jak chcemy podejść do
tego importu. Także polecam sobie
poczytać, jak dokładnie ma być to
sformatowane. Następnie klikamy import i
wala. I tak naprawdę to jest tyle.
Będziemy musieli poczekać chwileczkę, aż
ten import przebiegnie pomyślnie. No mi
trwał taki import do około 40 minut, ale
też mam bardzo rozbudowaną tą wiedzę, tą
bazę wiedzy. I teraz co jeszcze można
ciekawego zobaczyć z poziomu obsydian?
Oprócz tego, że mam tutaj te notatki,
mamy coś takiego jak otwórz podgląd
grafu i to jest właśnie to, co jest też
przewagą obsydiana. a mianowicie nie to,
że mamy jakiś tam śmieszny wizualny
podgląd, ale to, że te notatki mogą do
siebie mogą się ze sobą łączyć, mogą być
różne nawiązania do różnych notatek. I
teraz widzimy takie pewne zbiory. Tutaj
mam różne
chociażby AI Toolkiit. To jest taki lead
magnet z różnymi narzędziami, które ja
stworzyłem. Taki przybornik z różnymi
narzędziami AI. I teraz jak kliknę sobie
w ten przybornik, to mam bazę ze
wszystkimi linkami różnych różnorakich
narzędzi. 409 pozycji. I teraz z poziomu
tego grafu mogę zobaczyć jakie konkretne
tutaj
notatki, jakie konkretne wpisy są z tym
połączone. Tak? Czyli jak przejdę znowu
do tego toolkitu, mamy przeróżne. Każda
kropka, każdy tutaj obiekt to jest
osobne, osobna jakaś notatka, tak? Czyli
włączam i mam podgląd danego widoku,
czyli y właśnie notatka z notion z
konkretnymi opisem, oceną tego
narzędzia, linkiem i tak dalej, i tak
dalej. Także to co chcę wam przekazać,
że to jest właśnie też potęga Obsydiana,
że jesteśmy w stanie budować przeróżne
powiązania pomiędzy naszymi właśnie tą
wiedzą, notatkami.
Ale żeby to było jasne, tutaj akuratnie
mam to zrobione z poziomu mojego notion.
Tutaj nic nie było modyfikowane, ale w
tym drugim y no w tym drugim obsydianie
tu jest te wszystkie powiązania pomiędzy
nimi, no są budowane ręcznie. Y może nie
ręcznie, tylko automatycznie.
Automatycznie przez Cloda.
Mianowicie mam tutaj mojego pomocnika w
terminalu i tutaj jestem w stanie
generować sobie po prostu przeróżne
przeróżne.
Możemy sobie zrobić nowy czat. Tak,
zrobimy sobie nowy czat. jestem w stanie
z tym voltem pracować. Tak, czyli
powiedz mi, czego dotyczy ten Volt? Tak,
czyli mogę śmiało cloda zapytać tutaj w
terminalu, z czym mamy do czynienia.
Tutaj po lewej mamy oczywiście nasze
folderki. Mam tutaj ROW, mam wiki, mam
personę, czyli też określoną określonego
siebie jako osobę, mój styl pisania,
tworzenia, żeby też Claud lepiej
zrozumiał jaką, w jaki sposób ja też
piszę moje notatki, żeby tworzył coś
podobnego na mój wzór. Tak, czyli mam
opisane pokrótce dedykowany research hub
o trzech głównych tematach. Obsyian,
clot code, no i też integracja pomiędzy
tymi dwoma narzędziami. No i też jest
prosta warstwa, czyli mamy row, czyli
takie miejsce, gdzie wrzucam wszystkie
źródła, jak idzie. Wiki to jest synteza
tej wiedzy. No i clot to jest cały
schemat, taka konstytucja naszego Volta,
czyli definiuje w jaki sposób te reguły
mają się zachowywać jeśli chodzi o
tworzenie tych notatek. I teraz jeśli
chodzi o samego podejście to Karpatiego,
ja troszeczkę mam to rozwiązanie
rozbudowane o różne tutaj integracje,
pluginy. Mam też tutaj różne
stopniowania tych notatek, czyli na ile
jest to źródło zaufane, na ile nie.
Natomiast tutaj nie będę się rozgadywał,
bo Krzysiek wam też trochę wytłumaczy
czym w ogóle jest ta koncepcja LLM wiki.
Ja tutaj tylko pokazuję wam jak to
wygląda u mnie tak domyślnie i tak na
szybciutko żeby pokazać jak to mniej
więcej może działać czyli wejdziemy
sobie do przeglądarki i mam przykładowo
jakiś filmik powiedzmy Carpaty Obsidian
Cloud Code tak czyli mogę sobie wrzucić
wyszukać jakiś link na przykład Obsydian
RCK tak i teraz klikając ten w ten
filmik biorąc link mogę sobie też śmiało
wziąć i albo skopiować link i wrzucić go
bezpośrednio
do obsydiana w ten sposób, czyli
bierzemy row, wrzucamy nowa notatka i
dajemy mu tutaj jakiś link. Mogę to
śmiało tak zostawić. I teraz o jakiś tam
filmik ety. Tak. I teraz co mogę zrobić
to powiedzieć mu ingestzuj
wiedzę. I co on zrobi to przeglądnie
sobie te surowe materiały. Część z nich
już po prostu większość z nich jest już
przetworzona, więc doszedła, doszła nowa
jedna jakaś notatka. I co teraz? Clud
zrobi to zobaczy jakie pliki nie były
przetworzone w mojej bazie wiedzy.
Wyłapie takie pliki, nawet jest ich
więcej, nie jedno, ale pięć. I teraz co
on zrobi? To te pliki sobie wyciągnie i
na bazie ich będzie mógł przygotować
właśnie tą wiedzę, syntetyzować te
notatki. Proszę bardzo. Znalazł pięć
różnych źródeł i teraz co mogę zrobić to
powiedzieć mu, mam ten filmik na
YouTube. Tak tutaj powiedzieć syntezuj,
syntezuj na razie tylko ten jeden tak
żeby się zajął tylko tym. Na razie nie
będziemy robić wszystkiego, żeby to
długo nie trwało. Ja działam na opusie.
Oczywiście tutaj do takich notatek
możemy śmiało wykorzystać jakiś model
typu sonet. będzie to na pewno
wydajniejsze. I co on teraz robi, to
wykorzystuje też skille, które ma pod
spodem do pobierania danych właśnie o
tym filmie i następnie przygotuje pewną
syntezę na bazie tych tej wiedzy, którą
ma i będzie ją aktualizował o te nowe
informacje z tej notatki. również jeśli
zauważy, że są jakieś sprzeczne
argumenty, to też jest w stanie tego w
tym wolcie mi to zaznaczyć, że coś jest
na przykład nieaktualne albo coś na
przykład tutaj ktoś pokazuje inne
podejście i teraz on też może rozważyć,
które podejście jest stosowne albo
zapytać się mnie, więc razem ze mną
buduję tą wiedzę. Tutaj też Krzyśku
możesz powiedzieć gdzieś tam swoje jakie
przemyślenie masz na ten temat, bo to co
też pokazał na przykład Karpati to ja
widzę tutaj pewien minus w tym wszystkim
to to, że to w sumie w każdym ragu to to
tak działa. Czyli jeśli dajemy jakiś
garbage in, czyli jakieś śmieci do
środka naszej bazy wiedzy, no to musimy
się liczyć z tym, że później garbage
out, czyli ta wiedza z różnymi błędami
może nam później ciążyć w tym naszej
bazie wiedzy. Także też trzeba mieć brać
pod uwagę co my w ogóle wrzucamy do tego
Volta. czy te dane, które wrzucamy są
poprawne, czy czy w ogóle wnoszą jakąś
prawdziwą wartość do tego Volta, czy są
jakimś śmieciem, który może nam
przynieść mniej korzyści, a bardziej no
zaśmiecić tą naszą bazę wiedzy. Tak to
takie to to możesz też Krzysiku
powiedzieć, czy z czymś takim się
spotkałeś. Ja tu tylko jeszcze zanim
oddam ci głos, bo będziemy się
przepinać, Krzysiek pokaże też to u
siebie już bardziej szczegółowo, jak to
można setupować. Yyy, mianowicie
dostałem informację, zanim syntetyzuję,
proszę bardzo, dostałem informację, dużo
tu pokrywa się z tym, co mamy. Czyli
Clod nie wrzuca tego bezmyślnie do
mojego obsydiana, do mojej tej takiej
biblioteki pamięci, wiedzy, tylko pyta
mnie czy w ogóle chcemy to wrzucić. Czy
widzisz tutaj cię coś ciekawego, co
moglibyśmy śmiało dodać. Tak, mogę mu
powiedzieć śmiało, że dwójka chce, żeby
stworzył osobną stronę Wiki. Wiki chase
AI to jest ten gość, który przygotował
autor tego filmu. I następnie
no właśnie na bazie tego będziemy mieć
też jakąś notatkę do tego filmu, ale
będzie to osobna notatka, która nie
będzie pokrywała się z innymi. Więc
wzbogacam istniejące strony o nowe
kleimy tutaj z Chaseu będzie dodawał z
tego filmu. I co się dzieje tu w tle u
góry po prawej, co możecie zauważyć, to
to, że co chwilę jak coś się edytuje w
moim wolcie, jak coś dodaję, czy też kod
zmienia, to co chwilę leci mi tutaj
aktualizacja z boku. A to z tego powodu,
że cloda ma ten projekt z Cloudem mam
też wrzuconego do Githuuba. Czemu? Bo
teraz za każdym razem jak robi się jakaś
zmiana od razu dostaję nową wersję na
GitHua i mogę ten projekt włączyć sobie
z poziomu telefonu, z poziomu innego
urządzenia, tabletu. Także ta baza
wiedzy jest ze mną w każdym miejscu, nie
tylko na moim komputerze. I myślę, że to
jest też bardzo ważne. No bo po co
tworzyć bazę wiedzy, która jest
niedostępna z innych miejsc, tylko z
naszego komputera. No jest to dosyć
karkołomne i też dodawanie takich
notatek do do takiej bazy byłoby na
pewno utrudnione. Więc ja mogę w takim
setupie dodawać sobie notatki równie
dobrze z poziomu mojego telefonu. E i
tutaj już jest dodawana notatka. Tylko
jeszcze pokażę na szybko jak to wygląda.
Czyli mamy wiki/arpaty llm wiki tak
czyli mogę sobie przejść tutaj po lewej
jak mam tego Volta do tej notatki tak i
tutaj poniżej gdzieś zaraz powinno się
pojawić to nawiązanie. Widzę, że jeszcze
się chyba aktualizuje. Dokładnie.
Jeszcze musimy chwileczkę poczekać, ale
on w różnych plikach, proszę bardzo,
dodał sobie te uwagi po prostu odnośnie
tego filmu. Także to też jest fajne.
Proszę bardzo. Obsidian webclipper,
czyli to jest notatka z samego tego
narzędzia, które też Krzysiek zaraz
pokaże do łapania różnych treści z z
przeglądarki, z internetu. Też dodał
sobie informacje o o tym chasie. Zaraz
to się powinno zaktualizować, będziemy
to widzieć. Także jeszcze chwileczkę
poczekajmy. A dokładnie to co ja
zrobiłem to to jest folder row, czyli to
są surowe dane. Więc ja nie chcę też,
żeby mojej wiedzy takiej podstawowej,
którą wrzucałem, żeby tu on robił jakieś
modyfikacje. Chcę żeby to były surowe
notatki, żeby w każdej chwili można było
do nich wrócić i zobaczyć, co jest bazą
do tych notatek zsyntetyzowanych przez
AI. To mi daje też pewne źródło
wiarygodności, że te notatki nie wzięły
się znikąd. I tu jak wrócę do Wiki, tu
już są stetyzowane notatki, więc tu
będziemy widzieć chociażby nawiązanie do
tego filmu. Proszę bardzo.
Tutaj mamy proszę bardzo. Chase AI. Jest
jakieś nawiązanie, decyzja. I tutaj
jeszcze jakbyśmy poszukali dalej to będą
pewnie nawiązania do innych plików.
Proszę bardzo. Mogę się pomiędzy nimi
przełączać i zobaczyć gdzie one mnie
dokładnie prowadzą. Tak więc jak wrócę
tutaj do mojej bazy wiedzy to też można
zobaczyć, czy ona się bardzo rozrasta. I
też ostatnia rzecz, którą jeszcze tutaj
dodam od siebie, to mam też logi, czyli
mój obsydian też z każdą zmianą zapisuje
co się wydarzyło. Mogę sobie wrócić i
zobaczyć dokładnie każdego dnia, co
doszło do moich notatek, jakie zmiany
poczyniliśmy, co zaktualizowaliśmy. To
jest też ważne, żeby mieć świadomość jak
ten VT się rozrasta i w którym miejscu
jesteśmy i też co robiliśmy wcześniej,
tak żeby nawet wyłapać potencjalne
jakieś błędy, a może chcemy coś
poprawić. To jest też bardzo ważne, żeby
widzieć jaki stan jest na dany dzień
tego naszego Volta. Także rozgadałem się
Krzyśku, także wybacz mi za to i no
chciałbym żebyś też pokazał perspektywę
ze swojej strony, bo też szczerze mówiąc
nie kontaktowaliśmy się między sobą,
jeśli chodzi o te projekty, które
dzisiaj dla was przygotowaliśmy. Także
dla mnie to też będzie ciekawe, jak ty
do tego podszedłeś.
Podszedłem w dość podobny sposób do
ciebie, bo też oparłem się o Karpatiego,
aczkolwiek nie modyfikowałem tak jak ty
to uczyniłeś. tylko przeszedłem to w yyy
powiedzmy jen do, ale wprowadziłem wiele
automatyzacji w tym procesie, które będę
chciał wam właśnie pokazać. Ale zanim
jeszcze do tego wskoczymy, to wielka
prośba do was.
Dajcie nam znać, czy to, co pokazaliśmy
do tej pory podoba się wam, czy widzicie
w tym wartość.
A jeśli tak, to bylibyśmy wdzięczni,
jeśli byście się odwdzięczyli subem,
lajkiem, komentarzem. to pozwala nam po
prostu dotrzeć do większej liczby osób,
a uważamy, że y to co pokazujemy na tych
warsztatach no naprawdę jest dobrej
jakości, a y tym bardziej, że jeszcze
realizujemy to na żywo, to tym bardziej
oczekujemy, że po prostu się
odwdzieńczycie, tak w postaci właśnie
tych subskrypcji, lajków.
>> Oczywiście przymuszamy, to jest wasza
dobra wola. Natomiast zapraszamy,
zapraszamy tutaj do lajkowania i też
komentowania, jeśli macie jakieś uwagi.
To też to, co ja powiem, to ja też w
ramach takiego bonusu, jak zostaniecie
na na do samego, wytrwacie z nami do
Q&A, to też z chęcią podzielę się
projektem, który przygotowałem do
zbudowania właśnie takiego Wiki od zera.
Mam przygotowany template tego, podobnie
jak działa takie moje wiki i
przygotowałem szablon, który będziecie
mogli sobie zaczytać do swojego cloda na
swój komputer i z nim zbudować takie
właśnie taką bazę wiedzy. Tam będziecie
prowadzeni za rączkę krok po kroku. O
czym chcecie tworzyć tą waszą wiki, ten
drugi mózg, z czego jak ma jaka jest
wasza persona, też będziecie mogli
opisać. To jest też myślę ważne do tego,
żeby wasz projekt i wasz AI też rozumiał
z czym ma do czynienia, z kim ma też do
czynienia.
Także też coś takiego podrzucę.
Natomiast to też dla wytrwałych, którzy
z nami zostaną, także to dopiero
później. Także Krzyśku też tutaj
zapraszam na pokazanie siebie też. Także
oddaję pałeczkę, oddaję ekran.
>> Mhm.
>> Jasne. Wielkie dzięki Krzychu, świetna
robota.
Mamy już też pierwsze sygnały, że jest
git. Jasne, że się podoba. Sub poszedł.
Wielkie dzięki.
Także tutaj sporo osób na czacie
jest zadowolona z tego, co dotychczas
pokazaliśmy.
Także nam
>> Pamiętajcie, że to co my pokazujemy, to
pamiętajcie, że to co my teraz
pokazujemy to chcemy wam pokazać pewne
możliwości jakie możecie zrobić z
obsydianem, co on daje realnie i nie
jesteśmy w stanie, że tak powiem,
pokazać tutaj tego setupu na żywo od
zera totalnego. Natomiast też to co
myślę to w ramach takich też materiałów
po warsztacie dostaniecie na pewno na
maila. O to się postaram. taką
podsumowanie z najciekawszymi linkami i
też nawet właśnie z no właśnie może z
tymi materiałami bonusowymi, o których o
których tutaj wspominałem przed chwilką,
żebyście mogli ruszyć swoim obsydianem,
jeśli wcześniej z nim nie pracowaliście
oczywiście, bo jeśli ktoś już działał,
to również będą ciekawe takejki i moje
uwagi, które ja też wprowadziłem w tym
wiki, bo to co ja tu pokazuję, to nie
jest taki klasyczny Karpati, tylko
trochę rozbudowany o moje potrzeby, bo
te wiki, które budujecie, te drugie,
drugie mózgi, że tak powiem, powinny być
dostos
jak najbardziej pod was. Każdy ma
troszeczkę inny styl pracy i myślę, że
to co też Krzysiu ty pokażesz, no to też
jest troszeczkę inne podejście.
Dokładnie, zgadza się.
Zanim jeszcze ja skoczę na swoją część,
którą chciałbym wam pokazać, to taka
mała przypominajka. Jeśli macie jakieś
pytania, to śmiało zadawajcie je na
poziomie czatu. Fajnie, jak jeszcze je
oznaczycie na przykład jako Q, czyli
jako question, to nam też to pomoże
później odpowiedzieć na te wszystkie
pytania, bo my oczywiście po naszej tej
części merytorycznej zostaniemy jeszcze
z wami przez jakieś 30, 40 minut, żeby
poodpowiadać na te wasze wszystkie
pytania i postaramy się no dość mocno
zaeksplorować te tematy, które będziecie
tutaj do nas rzucać. I jeszcze takie
pytanko do was, jakbyście mogli się
podzielić na czacie. Czy ktoś w ogóle
już zbudował swój second brain i czy
dowozi on wartość.
Dobra, ja już się tutaj przepinam na
prezentację.
Okej.
Miałem dopiero zamiar budować. Fajnie
tutaj dostaliśmy komentarz od Nexora.
Myślę, że też z tymi z tym szablonem
będzie cię o wiele prościej ruszyć po
prostu i zbudować taki pierwszy swój
second brain, bo chodzi o to, żeby
ruszyć i zacząć coś z tym robić, a nie
czekać, nie oglądać setki tysięcy
tutoriali, tylko już zacząć z tym
działać i zobaczyć jak wam się z tym
pracuje, bo ja widzę dużo benefitów
chociażby z tym, co powiedziałem
wcześniej, czyli danie dania drugiego
życia swoim starym notatkom, do których
nie zaglądacie, bo no nie macie na to
przestrzeni albo no nie chcecie tym
zarządzać od nowa, od zera budować,
tylko możecie to też do tego
wykorzystać. ća czy jakiegoś innego
asystenta, który będzie z waszym
obsydianem mógł współpracować i wyciągać
tą wiedzę, syntetyzować.
No widzę tutaj, że już pierwsze osoby
dzielą się informacjami, że właśnie są
na etapie tworzenia swoich second
brainów.
O, kolejna osoba też dzisiaj już tutaj
działała, więc to nas tym bardziej
cieszy.
Dobra, jeszcze w ogóle taki mały news,
bo odpaliłem przed chwilą nową sesję CL
Coda, a tutaj
>> 47
>> mała niespodzianka 47 wyszedł,
>> także będziemy mieli okazję dzisiaj na
żywo przetestować od razu opusika 47.
Zobaczymy jak sobie będzie radził z tymi
notatkami.
Natomiast tak jak Krzysiek wam obiecał,
że rozszerzę wam trochę koncepcję
Karpatiego, o co w ogóle w tym wszystkim
chodzi. Więc tutaj wam
pokażę w jaki sposób Karpati podszedł do
tej koncepcji,
bo wiecie,
Andrej Karpati jest tak naprawdę jednym
z ojców tego nowoczesnego AI i on
właśnie wpadł na bardzo prosty pomysł,
jak używać LLM do zarządzania wiedzą. E,
Krzyśku, możesz na pełny ekran, bo to
jest faktycznie, żebyś nawet przybliżył
ten właśnie diagram, nawet na pełny
ekran idę, to też super.
Świetnie, od razu lepiej.
>> Jasne. Tutaj jak najbardziej tutaj
otworzymy.
Dobra, powinno teraz być już widoczne
dla was. Yyy, ogólnie yym
jeśli chodzi tutaj o tą całą ideę,
większość ludzi używa AI jak
wyszukiwarki. Z taką ideą w ogóle
wyszedł Andrej Carpati. M, masz po
prostu pytanie, dajesz mu jakieś
dokumenty, on ich szuka. Za każdym razem
od zera. Jakbyś za każdym razem
tłumaczył nowej osobie całą historię
powiedzmy swojej firmy. Tak. A co gdyby
zrobić to inaczej? I z takim pytaniem
wyszedł właśnie Andrej Karpati
i tu pojawiła się jego analogia. Wyobraź
sobie, że twoje notatki, jakieś
artykuły, PDFy czy nawet kod źródłowy, z
którym pracujesz jest surowy,
nieprzetworzony dla człowieka do
czytania, ale LLM jest właśnie takim
kompilatorem,
który
jest po prostu takim naszym
kompilatorem.
który przetwarza go raz i produkuje coś
gotowego do użycia. I właśnie tym
elementem do użycia, jak tutaj nazwał
swoim tym całym koncepcie jest właśnie
to wiki, czyli taki skompilowany już
program gotowy, poukładany z linkami
między tematami. Nie kompilujesz go za
każdym razem, kiedy chcesz go uruchomić.
Czyli mamy już gotowe, przetworzone
notatki. No i kolejnym jakby takim
etapem to jest taki test su, który
zaproponował, czyli tak zwany lint,
jest to taka kluczowa zmiana, tak? Za
każdym razem
jak zapraszamy tego naszego test sua, to
on po prostu sprawdza, czy nie mamy
jakiejś brakujących linków, może trzeba
coś uzupełnić, może są jakieś
sprzeczności. brakuje jakieś informacji,
więc to pozwala nam utrzymać ten nasz
second
w ryzach. No i takim ostatnim elementem
jest już ten runtime, którym on tak
ładnie to nazwał. I to jest właśnie
kluczowa zmiana, że zamiast za każdym
razem szukać w dokumentach, masz gotową
bazę wiedzy, z którą AI zbudował dla
ciebie i możemy sobie z nią rozmawiać.
Więc w tej fazie po prostu mamy już taką
typową interakcję, eksplorację tego, co
zbudowaliśmy. No i też możemy sobie to
podejrzeć właśnie z poziomu takiego graf
view.
A co ważne, Karpati tutaj też zauważył
pewne problemy, że to słabo się skaluje,
ale o tym wam opowiem trochę później
i może byśmy już tutaj przeszli od razu
do jakiś przykładów,
gdzie ja już tutaj mam zbudowaną tą całą
strukturę. Jak możecie zauważyć, mam
tutaj ten właśnie mój Fordel Row, który
zawiera te nieprzetworzone notatki oraz
tą całą Wiki, która już ma skompilowaną
wiedzę za pomocą LLMA.
I przejdźmy może do jakiś takich
pierwszych już przykładów demo, gdzie
pokażę wam właśnie użycie webcpera,
którego Krzysiek wcześniej już używał.
Załóżmy, że chciałbym sobie dodać ten
materiał wideo do moich notatek, więc
klikam sobie w webclickera i daję add to
obsidian. I teraz jak widzicie, otworzył
mi się ten obsydian, a w tle wykonuje
się pewna magia, bo jak wcześniej
wspomniałem, ja dodałem sobie kilka
automatyzacji. Jak tutaj już możecie
zobaczyć, została dodana cała
transkrypcja tego materiału, z tego
filmu na YouTubie.
która trafiła bezpośrednio
do moich tutaj notatek,
które mam je tutaj w videos, czyli mamy
dowody na życie poza ziemią. Taki dość
kontrowersyjny temat.
Natomiast
załóżmy, że też mamy jakieś materiały,
które nie wiem, przechowujemy na
przykład w postaci
PDFów.
Więc ja mam tutaj taki w tej mojej
strukturze katalog na PDFY, więc wrzucę
sobie tutaj plik z PDFem
i za chwilkę powinna znów się wykonać
pewna magia, gdzie tutaj do folderu z
przetworzonymi tymi
PDFami powinien pojawić mi się dokument
markdowny, w którym mam dokładnie
odwzorowaną tą strukturę tego PDFa.
To chwileczkę potrwa, bo jest to
przetwarzane przez model lokalnie u mnie
tutaj na komputerze.
Aczkolwiek za chwilkę wam
opowiem w jaki sposób w ogóle zbudowałem
tą całą architekturę, w jaki sposób te
automatyzacje się tutaj wykonują.
Także jeszcze chwileczkę, musimy się
uzbroić w cierpliwość, a ja w
międzyczasie pokażę wam jak w ogóle
wygląda ten dokument. Oczywiście
to jest wygenerowany na potrzeby tego
warsztatu, więc te wszystkie dane są
fikcyjne. Więc mamy taki dokumencik,
który jest umową o doradztwo
strategiczne w zakresie AI.
że wskoczmy sobie z powrotem do tutaj i
jak widzicie mam już odwzorowany ten
dokument zapisany całkowicie w formacie
markdowna.
Więc dokonaliśmy sobie tego dokumentu.
Nie stoi też nic na przeszkodzie, żebym
wziął na przykład
dokument, który jest obrazkiem.
Tak, mam akurat ten sam dokument, ale
zapisany już w formacie JPG,
więc jeśli sobie znów go przerzucę tutaj
do notesów,
notes, no tutaj. Dobra,
pyk.
Ojoj. A widzicie, mi wrzuca tutaj, a nie
tu, gdzie bym chciał. Dobra, to zróbmy
może na razie tak.
To co jest myślę Krzyśku ważne to żeby
wybrzmiało tutaj no bo okej no Clot sam
w sobie też umie czytać różne dokumenty
natomiast to co ty zrobiłeś to
przygotowałeś narzędzie które taki
przepływ że tak powiem przetwarzania
tych dokumentów że on nie leci przez te
modele chmurowo masz model lokalny który
trawi ci ten dokument i później te dane
jest w stanie zapisać gdzieś w projekcie
na przykład jakieś najważniejsze
informacje tak To to jest myślę, że
ważne do zaznaczenia, czyli to nie jest
taka standardowa ścieżka, no bo też no
nie polecałbym nikomu wklejać jakiś
danych poufnych umów i tak dalej
bezpośrednio do cloda. Także tutaj to co
Krzysiek zrobi pod spodem to właśnie ten
cały pipeline lokalny.
>> Tak. Ja za chwilkę tutaj rozszerzę
dokładnie jak ta architektura działa. M
bo ja za chwilkę tutaj też zapuszczę
pewne zadania do tego modelu, które będą
trwały sobie kilka minut, a w
międzyczasie będziemy mogli sobie
rozwinąć te wszystkie koncepcje jak
działają te w ogóle automatyzacje. Ale
jak widzicie ta ten dokument w postaci
JPG został już też przetworzony, czyli
ja nie muszę wykonywać żadnych akcji. po
prostu wpada mi tutaj dokument, czy to z
pomocą webca, czy wrzucam manualnie
jakiegoś PDFa, PNG, cokolwiek. Wszystko
jest automatycznie przetwarzane.
Dobra. M zanim jeszcze przejdę do
wytłumaczenia tej całej architektury,
jak to zostało w ogóle zbudowane, jak to
się dzieje tam pod spodem, to
chciałbym sobie porozmawiać teraz z tymi
dokumentami, bo wrzuciłem sobie właśnie
ten film
z YouTubea między innymi i tak dalej i
mamy tutaj kilka mamy
tutaj do dyspozycji kilka takich
elementów
Jeśli chodzi o operacje w kontekście
w kontekście właśnie tego całego mojego
seconda wzorowanego na Karpati możemy
mieć tak zwany ingest, czyli to są takie
interaktywna dyskusja z tym moim
z moimi źródłami, który czyta właśnie
moją tą wiki ten indeks, sprawdza, czy
zostało to już przekompilowane.
Następnie mogę sobie z nim porozmawiać,
jak to w ogóle działa i tak dalej. No i
w międzyczasie tego wykonania tego
ingesta jest realizowana właśnie ta cała
kompilacja, która trafia do tego
katalogu wiki
i mogę też sobie normalnie rozmawiać
później z tymi notatkami. Mogę wykonywać
tego linta, o którym wcześniej właśnie
wspominałem, czyli tak zwany ten health
check naszej Wiki, który sprawdza, czy
nie mam jakichś uszkodzonych
Wikilinksów,
czy nie ma jakiś brakujących backlinków.
czy nie wiem jakieś sprzeczności
brakujących stron, cokolwiek.
Więc do kolejnych tutaj jeszcze operacji
za chwilkę wrócimy, ale właśnie
wykonajmy sobie teraz tego ingesta, więc
porozmawiajmy sobie tutaj z tym naszym
teraz modelem.
Także pierwszy taki teścik na żywo,
jeśli chodzi o tego naszego opusa. Więc
ja mam przygotowane w ogóle już takie
komandy i skillsy. Ja akurat mam tutaj
komanda, który kompiluje tą wiedzę. Ja
sobie go mogę teraz wybrać i jeśli
wskażę mu po prostu jako new, to on
tylko weźmie wszystkie te nowe,
które
które źródła się pojawiły. Więc za
chwilkę opusik powinien mi zwrócić
jakie rzeczy pojawiły się w row. Jak
widzicie, on już tutaj sobie zaczyna
indeksować, że tu jest właśnie ten
przegląd ofert, czyli ten mój PDF jako
notatka,
ten mój JPEG
też powinien za chwilkę sobie
przetworzyć. O, widzicie. M a jeśli w
układzie słonecznym coś tam, czyli już
po prostu te materiały wideo, które
zostały w tym rowone,
one są już teraz przetwarzane przez
model
w ramach tego ingesta i on za chwilkę
będzie tutaj z nami rozmawiał, czy te
źródła chcemy jakoś pogłębić
i tak dalej.
O, i widzicie, on już właśnie teraz
przeczytał i okazuje się, że w tym moim
row mam aż pięć różnych źródeł.
I on w tak w skrócie nam opisuje, że do
tego mojego row wskoczyła właśnie jakaś
tutaj umowa, wskoczył jakiś tutaj
materiał dotyczący astronomii, czy jeśli
tam w układzie słonecznym mamy tam
jakieś sądy obcych. Mm, skoczył też
materiał między innymi tutaj Krzyśka
Bohaczyka yyy clot za darmo, do którego
was oczywiście zachęcam obejrzenia, bo
świetny materiał Krzyśkowi wyszedł. I
yyy kolejny materiał, czy mamy dowody na
życie poza ziemią, czyli ten, który
właśnie wrzucałem w ramach tego
materiału. Tak. No i teraz yyy strategia
kompilacji i mam tutaj yyy w jakim
kierunku chcę tutaj pójść czy PDF, jpg
jako jeden wspólny mnie wykrył, że to są
te same, stwierdził, że tutaj mamy
jeszcze dwa widea z astronomii i tak
dalej, więc ja mogę mu powiedzieć, że
weź mi teraz tylko skompiluj te źródła
związane z tymi filmami wideo, tak o
astronomii.
Weź mi teraz skompiluj te źródła
związane z astro.
Także dokonujemy sobie teraz tej
kompilacji
i ten etap trochę potrwa, więc w
międzyczasie
przejdziemy sobie do wytłumaczenia tej
całej architektury, jak to zostało
przeze mnie tutaj zbudowane.
mianowicie całość tutaj opiera się
o kilka takich mechanizmów
i pierwszym z nich są hooki, czyli jest
to mechanizm wbudowany bezpośrednio w
cloud coda i te hooki w zależności jaki
wybierzemy są uruchamiane
albo przed wykonaniem jakiejś komendy,
po zakończeniu jakiejś komendy.
czy też po prostu możemy je
wykorzystywać nawet w ramach skryptów
pisanych tutaj oczywiście przez koda
jakiś bashowych, powershellowych i tak
dalej. I ja na przykład mam kilka takich
przygotowanych już
rzeczy, jeśli chodzi o hooki i między
innymi jednym z takich hooków
jest start session start. Tak. I on jest
wykonywany, co ciekawe, raz w nocy o
23:00, czyli każdego dnia o 23:00 te
wszystkie notatki, które trafiają do row
kompilowane
do wiki.
Jest to o tyle fajny mechanizm, bo ja
sam nie muszę wchodzić i rozmawiać teraz
z tą
z tą z tym moimi źródłami,
tylko dzięki temu zyskuję e na przykład
jak rano sobie usiądę, że mam wszystkie
te źródła już ładnie przerobione i
nieważne czy ja tam wrzucę PDFa, wrzucę
PNG, czy wrzucę jakieś linki do filmów
na YouTubie, wszystko zostanie
przetworzone, bo jak już wcześniej
widzieliście jest tutaj właśnie taka
automatyzacja jak file system watcher.
Jest to zbudowany powersellowy skrypt,
który tak naprawdę zasadza się na
przykład na ten row videos
katalog i on śledzi. Jeśli pojawi się
jakiś w nim nowy plik, to automatycznie
wykonuje transkrypcję. No i też to
zostało zrobione w taki sprytny sposób w
moim przypadku y że w pierwszej
kolejności, jeśli jest to materiał y na
YouTubie to pobieram bezpośrednio z
YouTubea napisy
za pomocą takiej biblioteki jak YouTube
DLP, ale jeśli nie ma napisów, to wtedy
wykorzystuje FBA, którym jest lokalny
model, czyli Whisper Large, który
pobiera sobie
pobiera
wróć. Pobieram se za pomocą tego właśnie
YouTube DLP materiał audio, a następnie
transkrybuję go za pomocą Wispera.
Dzięki czemu pobieranie tych
transkrypcji,
materiałów z YouTubea nie kosztuje mnie
nic. To jest po prostu zero tokenów, bo
wykorzystuję gotową bibliotekę lub
lokalny model do tej transkrypcji. Tak
samo jeśli wpadnie mi plik MP4 czy jakiś
inny format wideo, to on jest wtedy z
automatu realizowany przez właśnie tego
Whispera.
I te wszystkie akcje wykonują się w tle,
zarówno OC i tak dalej. I w przypadku
OCRA wybrałem dość taki ciekawy model.
mianowicie jest to GLM OCR. Jest to
model, który
według benchmarków, o ile można im
wierzyć,
jest dużo lepszy niż nawet taki Gemini 3
Pro, jeśli chodzi o kilka benchmarków,
wypada dużo, dużo lepiej, więc czy nawet
taki GPT 5.2. Więc to jest naprawdę
fajny, solidny model i jak możecie
zauważyć jego rezultaty no są naprawdę
bardzo fajne, bo jak sobie przejdę tutaj
do tych proceed to a bardzo fajnie sobie
poradził choćby z tym dokumentem.
Dobra, trochę się rozgadałem o tym, o
tych hookach, więc
skąd w ogóle biorą się te źródła? Warto
sobie odpowiedzieć na takie pytanie.
Więc jeśli chodzi o te źródła,
to mamy tak naprawdę
kilka tutaj opcji. Pierwszą z nich,
którą wam pokazałem wcześniej jest
Obsidian Web Clipper, czyli po prostu
wchodzę sobie na jakąś stronę i mogę
zapisać czy to jakiś artykuł blogowy,
który leci do row articles, albo jakiś
link z YouTubea, który leci do row
videos,
jest zapisywany, albo po prostu
manualnie mogę sobie przerzucać te
wszystkie pliki tag. Wcześniej też
zresztą to zrobiłem w przypadku tych
umów czy obrazków, które lecą do
konkretnego folderu i z automatu za
pomocą właśnie tych watcherów,
które są uruchomiane przez hooki
są natychmiast
transkrybowane, oceowane i tak dalej.
Następnie właśnie jest wykonywany ten
preprocessing, o którym
kilka chwil wcześniej wam opowiedziałem,
czyli odpalają się watchery i robimy OC
obrazków czy jakieś transkrypcje
materiałów za pomocą właśnie tego
YouTube DLP czy nawet Whispera, jeśli to
splick audio. No i następnie jest
wykonywana kolejny etap i ten etap to
jest tak naprawdę
właściwie ten kompilator, o którym mówił
Karpati, czyli LM bierze przygotowane
źródła i kompiluje z nich
z nich Wiki. Ale mamy trzy sposoby, żeby
to w ogóle
uruchomić, tak? Bo znaczy mamy takie
trzy m etapy, których się tutaj dzieją,
czyli mamy tą takie syntezę tej wiedzy i
tworzenie tych wikilinksów, o których
wam Krzysiek tam wcześniej mówił, czyli
te połączenia między tymi wszystkimi
elementami.
generujemy backlinki, czyli takie
powiązane sekcje,
na podstawie których tworzy się graf
wiedzy, który wam też Krzysiek wcześniej
pokazał. No i mamy też taką jakby taki
element encyklopedii,
czyli system po prostu pokazuje jakby
koncept, nie wiem, choćby tej strony
podzielony na jakieś punkty, detale,
przedstawiający jakieś kluczowe wnioski
No i te tryby są uruchamiane
na wszelaki sposób, bo mogę uruchomić
sobie coś ręcznie, czyli tak jak teraz
tego ingesta sobie uruchomiłem,
czyli po prostu robię slash ingestowane.
Natomiast ja mam jeszcze te hooki, o
których wam wcześniej wspominałem i
właśnie mam tutaj takiego hooka, który
nazywa się Session Start. Może trochę
niefortunna nazwa, ale on generuje mi
właśnie taki ingest o 23:00 każdego
dnia,
który jest kompilowany właśnie do tego
wiki
i to jest właśnie ten cały chromej job.
Dobra, kolejny, czyli jak już ten LM
compiler sobie zadziała,
to mamy tutaj w końcu lądujemy właśnie w
tym całym naszym wszystko to ląduje w
tym naszym wiki i jest to właśnie tak
ten skompilowany program według analogii
Karpatiego i mamy tutaj strony
źródeł, czyli takie krótkie podsumowania
każdego artykułu, PDFa, transkrypcji, co
tam było, po co to czytaliśmy.
Mamy też y jakieś takie koncepty m
stron, czyli jeden temat, jedna strona,
jakieś embeddigi, ragi, fine tuningi,
każdy temat ma jakby swoją tutaj stronę.
No i mamy też generowane te esencje,
tak? Czyli tutaj możemy mieć na przykład
jakieś konkretne osoby, firmy, projekty,
które pojawiają się w tych naszych
materiałach. No i mamy jeszcze ten cały
indeks,
czyli to jest taki taka jedna strona,
która zbiera wszystko. To jest pierwszy
plik, który LM otwiera, kiedy zadajesz
jakieś pytanie.
No i następnie w ramach tego wiki
możemy sobie
robić tak naprawdę trzy rzeczy. Czyli
możemy yyy zadawać pytania, czyli
dostajesz odpowiedź synteyzowaną na
podstawie tego tej naszej Wiki. M nie z
tych dokumentów już skompilowanej
wiedzy, ale właśnie yyy z tej takiej
syntezy w ramach Wiki. Możemy też sobie
sprawdzać, robić linty, czyli możemy
sprawdzać tą naszą Wiki, czy ona jest
spójna, czy nie ma jakichś zepsutych
linków, osieroconych stron, sprzeczności
między artykułami.
M. No i możemy sobie wykonywać jeszcze
polecenia typu ingest, daily i tak
dalej. Czyli na przykład mam też tutaj
takiego komanda, który y przygotowuje mi
takie m codzienne podsumowanie tych
notatek. No ale teraz weźmy sobie
przejdźmy może do tych
mementów w ramach tej Wiki, żeby
zobaczyć jak to zostało tutaj
wygenerowane, bo jak widzicie tutaj ta
operacja trwa już 10 minut. i jeszcze
pewnie z jakieś dwie, trzy minutki
potrwa, zanim się to skończy, ale możemy
sobie już w międzyczasie zajrzeć do
rzeczy, których tutaj miałem. No i tutaj
są właśnie te nasze koncepty,
czyli widzicie, że tu są jakieś czerwone
karły i tak dalej, czyli mamy tworzone
notatki na podstawie każdego elementu,
który jest
w naszym źródle. Tak? Czyli jeśli
wrzucamy jakiś materiał o yy jakiś
gwiazdach, no to jeśli pojawiło się
jakieś stwierdzenie o czerwonych karłach
czy na przykład czerwone nad olbrzymy,
no to m każdy z takich ważnych pojęć
zostaje przygotowany jako taka notatka e
przedstawiająca ten główny konceptth.
Mhm. Mamy tutaj właśnie te entities i
tak jak wam wspomniałem to mogą być
osoby, firmy i tak dalej. I na przykład
mamy tutaj A ninjas, mamy tutaj choćby
astrofazę, jeśli chodzi o te materiały
związane z
z astronomią.
Mhm.
Mamy tutaj właśnie te sources
m, czyli już te nasze takie przetworzoną
syntezę tych naszych notatek.
No i mamy ten indeks, który przygotowuje
taką listę tych wszystkich materiałów,
jakie znajdują się w tych naszych
źródłach. Także tutaj troszeczkę ich
mam, jeśli chodzi o source, jeśli chodzi
o entities i jeśli chodzi o koncepty. O,
jak widzicie właśnie tutaj Cloud już
skończył pracę nad skompilowanymi
źródłami. Jak możecie zauważyć, miałem
tutaj dwa pliki wideo
i na podstawie tych dwóch plików wideo
zostało stworzonych aż 21 konceptów
i między innymi tu jakiś paradoks ten
przepraszam biostruktury,
jakieś
technosygnatury,
egzoplanety i wiele
wiele podobnych rzeczy. M. No i tutaj
zostały dwie encje przygotowane i tymi
encjami jest akurat autor astrofazy
czy autor paradoksu tego Fermiego. Więc
tutaj to wszystko zostało ładnie
przygotowane. Mamy też opisane
to wszystko w w metadanych, czyli
trafiło do indeksu naszego, trafiło do
wiki. Więc jeśli możemy sobie przejrzeć
ten nasz log też mamy tutaj informacje
co, kiedy gdzie trafiało, czy to były
jakaś inicjalizacja wiki, czy INGES, czy
rozmowa i tak dalej.
W ramach indeksu też trafił ten
materiał.
Trafiły te wszystkie materiały.
Dobra. No i możemy sobie teraz rozmawiać
z tymi naszymi materiałami. Mogę się
zapytać o jakąś rzecz, na przykład czym
jest paradoks Fermiego
i te nasze wszystkie rzeczy mogą trafiać
później do do tego Wiki jako unswers,
czyli po prostu zachowujemy później też
wszystkie te nasze rozmowy z tym naszym
naszym second brainem. No i tutaj mamy
opisaną właśnie ten paradoks. W takim
wielkim skrócie. Mamy też główne klasy
odpowiedzi, tak, na podstawie jakich
tutaj dokładnie materiałów, jakich
hipotez, na przykład ciemnego lasu czy
jakiegoś kosmicznego zo i tak dalej, to
zostało tworzone.
Oczywiście możemy też z tymi notatkami
jeszcze pracować na zasadzie
mogę sobie sprawdzić jakie są taski.
Więc to jest taka już ostatnia rzecz.
którą chciałbym wam dzisiaj pokazać.
Czyli na podstawie tych moich notatek
mogę poprosić jeszcze model, aby
przejrzał, czy nie ma tam jakiś action
itemów. Więc tutaj już sobie zapuszczam
to.
A w międzyczasie, kiedy tutaj czekamy na
odpowiedź, czy mamy tu jakieś zadania,
ja jeszcze bym wskoczył do ostatniej
rzeczy,
jeśli chodzi o
te diagramy, które dla was
przygotowałem.
O czym warto jeszcze pomyśleć, bo
koncepcja
Karpatiego
średnio się skaluje. Tam zresztą Andry
Carpati o tym wspomina, że w zależności
od jakiego modelu, jakiego rodzaju masz
notatki, to możesz efektywnie za pomocą
takiego clot codea czy innego, innej
sieci agencyjnej przetwarzać od 100 do
nawet 2000 notatek, ale co później, bo
one się już przestają mieścić w
kontekście i tak dalej. Dlatego
warto też pomyśleć nad tym, aby
rozbudować tą naszą bazę wiedzy o kilka
kolejnych elementów, czyli na przykład
przygotowanie raga, o którym Krzysiek
mówił. I fajnie się tutaj może sprawdzić
taki
yyy
multimodalny rak przygotowany choćby
przez Googlea, czyli tam Gemini
Multimodal RCK, który jest w stanie
przetwarzać nasze wideo, obrazki, teksty
i tak dalej, dzięki czemu będziemy mieli
zaindeksowane i będziemy mogli
wykorzystywać tak zwany semantic search
do zapytań o naszej całej bazie.
Warto jeszcze tutaj taki nasz second
brain według mnie rozszerzyć o pewne
integracje, czyli na przykład dać dostęp
do skrzynki, czy to Gmaila, Outlooka,
dodać na przykład dostęp do kalendarza
czy dostęp do jakiejś komunikatorów, z
których korzystamy, typu Slack, Teamsy,
może nie wiem, pobieranie jakiś
newsletterów, RS feedów. Ja tylko
Krzyśku powiem jedną rzecz, że myślę, że
to jest właśnie największa przewaga
budowania takiego takiego lokalnego, że
tak powiem, second braina, to to, że
będziemy mogli właśnie go zintegrować z
naszymi narzędziami, które używamy na co
dzień. No bo po co nam taki second
brain, do którego tak naprawdę będziemy
musieli wszystko, że tak powiem,
wprowadzać ręcznie, łopatologicznie. No
to jest mało, że tak powiem, łatwe do
zarządzania i utrzymania w dzisiejszym
świecie, który jest mega zagoniony i
chcemy wszystko robić szybko, sprawnie.
No i niestety gdzieś to nam, że tak
powiem, takie przygotowanie, zbieranie
tej wiedzy ucieka. Także to co mówisz
Krzyśku jest mega fajne i ja też tak w
ramach swojego prywatnego jednego z
Voltów zrobiłem to zrobiłem integrację
nawet z Gmailem. Tam nie muszą być
jakieś duże uprawnienia. Chodzi o samego
reada, czytanie jakiegoś konkretnego
taga, tak? Czyli na przykład newslettery
i może mi ściągać taką wiedzę i sam się
aktualizować, co nie? Czyli ja nie muszę
nawet gdzieś tam yyy go promptować ani
mu, że tak powiem, dostarczać te
materiały ręcznie, tylko można
zautomatyzować ten proces właśnie przez
takie różne narzędzia, co nie? To jest
świetne.
>> Mhm. Okej.
Jaż tutaj kończąc, o co warto jeszcze
rozszerzyć to no jakieś też pewnie do
task managementu narzędzia
czy na przykład jakieś API czy
automatyzacje, tak? Bo często może
korzystamy z jakiś, nie wiem, naenów,
zapierów, może mamy jakieś customowe
serwery NCP, może chcemy se wysłać
jakieś powiadajienia, alerty, no
cokolwiek, bo wtedy budujemy takie
narzędzie, które przykładowo
na podstawie, nie wiem, notatki z
rozmowy z klientem może przygotować nam
już drafta maila, tak, którego sobie
sprawdzimy i ewentualnie poprawimy i
wyślemy do niego.
możemy na przykład na podstawie tej
notatki zaplanować dalsze kroki, czy na
przykład wystawić spotkanie w
kalendarzu, tak, które będzie followupem
do tego pierwszego. Możemy powiadomić na
Slaku nasz team, więc to naprawdę
później na podstawie tego second braina
możemy budować taką fajną machinę, która
może zarządzać czy to naszym życiem
prywatnym, czy firmowym.
I
w międzyczasie właśnie Klaudiusz
skończył przetwarzanie i on zobaczył, że
w moich notatkach jest transkrypcja
rozmowy. Tak, mamy tutaj taką fake
transkrypcję rozmowy o wdrożeniu AI i ta
rozmowa była między Krzyśkiem a Markiem,
która była tam 14 kwietnia. No i
kontekst właśnie wdrożenie AI w ich
firmie. No i wywnioskował z tych moich
notatek, że do piątku 17 no miałem
wysłać temu Markowi ofertę,
odebrać od Marka jakieś 50 próbek
faktur, PDFów i oczywiście tutaj nie
będę się przechodził przez to wszystko,
ale koncepcja wam powinna być doskonale
już
nakreślona. No i tutaj mamy po prostu
przygotowane teraz taski,
które mógłbym
sobie wrzucić do jakiegoś narzędzia typu
toistira czy czegokolwiek tam używam.
Dlatego też jak widzicie ja nie tylko
muszę rozmawiać z tymi notatkami, ale
przy odpowiednich integracjach
z narzędziami czy jakimiś APami i tak
dalej.
Możemy też
realizować jakieś konkretne action
itemy, czyli tak jak wcześniej
wspomniałem, pisać jakiegoś drafta
maila, napisać do zespołu, przekazać
jakąś wiadomość dalej na podstawie
notatki, czy tak jak teraz w tym
ostatnim przykładzie, który wam
pokazałem, przejść do
na przykład sprawdzenia, czy w moich
notatkach nie ma jakieś właśnie action
itemów, czyli coś, co ja powinem zrobić,
czyli jakieś taski. I to jest według
mnie naprawdę bardzo ciekawe
ciekawa rzecz, jeśli chodzi o ten second
brain. No i w zasadzie to jest tyle, co
dla was dzisiaj tutaj przygotowałem.
A
>> jak wam się w ogóle podobały, czy nie
było za dużo, że tak powiem, no bo
staramy się tutaj szanować wasz waszą
uwagę i też to, żeby nie przedłużać tych
warsztatów.
>> Krzyśku, twojej kamery nie widać.
Tak, tak, tak. Okej, widzę już się
musiała wyłączyć. Już uzupełniam,
już naprawiam. O, proszę bardzo.
>> Tak jak Krzysiek wspomniał, no
staraliśmy się
zrobić naprawdę taką
syntezę tej wiedzy, żeby pokazać wam
mniej więcej cały taki zarys, bo
oczywiście w ramach takiej godzinki czy
tam tych 70 minut jest bardzo ciężko m
tutaj przedstawić te wszystkie koncepty
i wejść w nie bardzo głęboko. Dlatego my
zrobiliśmy taki big picture tego, jak my
podeszliśmy do budowania tego second
braina. Oczywiście za chwilkę też
przejdziemy do tej sesji z Q&A,
ale chciałbym tutaj jeszcze Krzyśkowi
oddać na chwilę głos, bo też
przygotowaliśmy dla was pewną tutaj
niespodziankę,
o której tutaj Krzysiek wam opowie. Więc
ja też tutaj jeszcze czekam, aż Krzychu
udostępni ekran.
>> Tak, tak, tak, już udostępniam. Tak, w
międzyczasie też możecie dać nam znać,
co w ogóle sądzicie o tym, co
pokazaliśmy. Czy podobało wam się? Może
macie jakieś pytania
do tej części, którą pokazaliśmy. Może
coś wymaga, nie wiem, rozszerzenia,
tak? Czy w ogóle już mówię, czy chce,
czy widzicie w tym potencjał na to, żeby
budować w ogóle taki second brain u
siebie?
Także tutaj też możecie śmiało śmiało
dać znać, a ja już się włączam też z
tym, co mam wam do pokazania, też z tymi
bonusami, które przygotowałem tutaj dla
was. To też śmiało chcę wam też pokazać.
Także oczywiście zadawajcie tutaj
pytania na czacie, bo za chwilkę
przejdziemy właśnie do tej części Q&A, w
której postaramy się zaeksplorować
wszystkie tutaj pytania, które
zadaliście dotychczas. No i liczymy, że
też
zaangażujecie się później bardziej w tą
naszą dyskusję, bo też chcielibyśmy z
wami jeszcze chwileczkę porozmawiać.
>> Tak, tak, tak, tak. Już, już śieszę w
ogóle, bo tak tutaj gdzieś tam
patrzyłem, y gdzieś tam czasami zerkałem
na czat, chociaż on bardzo szybko nam
tutaj uciekał, a mianowicie widziałem,
że ludzie się pytali o to, no dobra,
pokazujecie tyle dużo ciekawych rzeczy,
ale jak to w ogóle, że no chcę coś
takiego zbudować, ale jak to zbudować?
Tak tu się widzę, że pojawiają te
pytania, jak w ogóle do tego siąść.
Także wiem, że to może być troszeczkę
przytłaczające, bo tych rzeczy jest
bardzo dużo. Także już udostępniam ekran
i też pokażę wam, co w ramach takiego
bonusu przygotowaliśmy dla was.
Tak.
O, proszę bardzo. Także to, co ja
przygotowałem tutaj w ramach z
Krzyśkiem, to taką trochę syntezję tego,
co dzisiaj yy omówiliśmy i takie
najważniejsze rzeczy. Tą instrukcję
tutaj, co mam w Notion. Oczywiście w
Notion, bo będzie mi tak proście
udostępnić tutaj tego przez obsydiana.
Wam nie daję tutaj dostępu do siebie do
obsydiana. Natomiast co tutaj
znajdziecie to na pewno krok po kroku
instalację obsydiana, zrobienie
pierwszego Vta, ale również i GitHua do
naszego projektu, który opisuje krok po
kroku jak można w ogóle takiego taki
projekt u siebie zbudować. Tutaj jest
rozpisane też krok po kroku jak
wyglądają te warstwy, jak wyglądają
operacje, czyli właśnie ingestów
Krzysiek, czyli dodawanie wiedzy, jak
wygląda query, czyli zadawanie pytania,
no i też lint czyli taki health check,
spójność naszej po prostu bazy, bo
oprócz tego, że dodajemy nowe rzeczy,
też trzeba po prostu tym sprytnie
zarządzać i aktualizować. To jest
totalnie normalne. To są też takie
bonusy, które ja też od siebie dodaję,
czyli taką customizację, czyli jeśli
chodzi o ile źródeł potwierdza chociażby
jakość yyy tej wiedzy, confidence, taki
score. Też mam tutaj świeżość tych
notatek, czyli kiedy były weryfikowane.
Możecie sobie śmiało poczytać i zobaczyć
jaką tutaj koncepcję ja na to przyjąłem.
Generalnie pomysł jest prosty.
Wgrywacie, pobieracie ten projekt u
siebie na komputer, wpuszczacie cloda i
on ma też tutaj plik Bootstrap, który
przeprowadzi was za rączkę krok po kroku
i wytłumaczy wam jak takiego Volta
skonfigurować pod wasze zadanie
konkretne. Tak czy uży jakiego używasz
AI, jak piszesz, jaki jest twój styl
pisania i też o czym jest wasz Volt.
Tak, bo wasz Vol może być typowo o, nie
wiem, o marketingu. może być Volt o
właśnie jakiś zbieraniu researchu czy
też może jakiś projekt wasz jeśli chodzi
o firmę to też można sprecyzować także
coś takiego dostaniecie i tutaj krok po
kroku będziecie mogli przez to przejść
mail już powinien u was wylądować
Krzyśku możesz też jakbym cię prosił
wysłałem ci na Discorda linka jakbyś
mógł też przy okazji wkleić na czat może
że mi się teraz szybciutko uda to zrobić
to też udało mi się nawet
>> nawet mi się udało także zostawiam linka
żeby nie było że że tutaj nagadaliśmy
się na szybko, a nie ma gdzieś tam tego
kroku po kroku, jak można z tym zacząć.
Oczywiście każdy może ten Volt zbudować
po swojemu, nie ma jednej idealnej
idealnego podejścia, więc polecam wam
poeksperymentować i zobaczyć co dokład
dokładnie można jeszcze tutaj ciekawego
zrobić. A jeśli nie do końca wiecie w
którą stronę pójść albo właśnie chcecie
być na bieżąco, ale tych informacji jest
bardzo, ale to bardzo dużo. Zresztą no
tak jak dzisiaj wyszedł nowy model Opus
47 przed warsztatem nie byliśmy w stanie
nawet jeszcze jego przetrawić. Ja tam
oczywiście jakieś wstępne research
zrobiłem, natomiast no jest tego bardzo
dużo. To co mamy z Krzyśkiem wam do
pokazania to mianowicie społeczność AI
Ninjas, którą rozwijamy już od jakoś
początku stycznia. Jest to miejsce,
które gromadzi właśnie osoby, które są
zajawione podobnym tematem, czyli
sztucznej inteligencji. I co tutaj
ciekawego można znaleźć, to warsztaty co
dwa tygodnie z ekspertami, które
prowadzimy, bibliotekę nagrań, czyli
można do wszystkich nagrań wrócić
śmiało, gotowe procedury, czyli jakieś
konkretne rozwiązania, wdrożenia, które
my robimy i się nimi dzielimy, jakieś
konkretne skille, czy tak właśnie nawet
to, co w ramach Obsydiana
przygotowaliśmy, to też dzielimy się w
ramach społeczności już bardziej
szerzej, że tak powiem. tam mamy więcej
przestrzeni na to, żeby poruszać te
wątki jako osobne lekcje. No i to też co
najważniejsze to to, że jesteście,
obracacie się między ludźmi, którzy no
również po prostu są zainteresowani
podobnymi tematami, chcą się rozwijać i
zgłębiać tą wiedzę. Tu są też różne
wycinki z naszych poprzednich
warsztatów, czyli chociażby
automatyzacja odpowiedzi email z
lokalnym modelem, czyli też takie fajne
rozwiązanie pod firmy, generowanie
kreacji, więc też wykorzystanie tego AI
do marketingu czy też generowanie wideo.
Tutaj jest są przeróżne tematy, nie
tylko programistyczne, tylko też dla
osób, które dopiero zaczynają i
chciałyby w ogóle wykorzystać ten
potencjał, jaki nam daje, bo daje bardzo
duży, ale trzeba to zrobić z głową. I
taka propozycja też dla was i oferta z
tego, że powodu, że wytrwaliście w ogóle
z nami dzisiaj, to najniższa okazja do
dołączenia, a mianowicie minus 50 zł
zniżki na dołączenie po prostu do naszej
społeczności. Jest to oczywiście pakiet
miesięczny, także nie chcemy wam tutaj
sprzedawać czegoś, z czego nie będziecie
mogli się wycofać powiedzmy za miesiąc,
dwa. Jeśli stwierdzicie, że to jest dla
was niewystarczające, to w każdej chwili
możecie zrezygnować. Y, także tym na
pewno się różnimy. Y więc no chcemy być
z wami szczerzy. Jeśli wam się podoba
to, co robimy i szukacie więcej takiej
wartości, no to też w ramach takiego AI
Ninja społeczności, zaraz pokażę też jak
mniej więcej to wygląda w środku,
będziecie mogli do nas dołączyć i z nami
po prostu przemierzać ten świat
sztucznej inteligencji. Więc to co tutaj
na stronie jest, ja też podrzuciłem
linki, to zniżka minus 50 zł. To jest
najniższa cena jaką mamy i podejrzewam,
że to będzie ostatnia taka duża
promocja. Mianowicie ten kod jest ważny
przez trzy miesiące, czyli jak raz
dołączycie to przez trzy miesiące macie
tą najlepszą cenę. Tu są trzy pakiety.
Pakiet najtańszy to jest 99 zł za
miesiąc. Macie dostęp do minikursów, do
biblioteki gotowych procedur, do
warsztatów co dwa tygodnie z ekspertami.
Mieliśmy tematy chociażby stworzenia
stron, które nie wyglądają jak AI slop,
czyli przypominające po prostu
wygenerowane z AI. Mieliśmy warsztat też
ze skrapowania, pobierania danych z
internetu, z różnych stron, także też
scrapowania, pobierania danych o
konkurencji i też warsztaty chociażby z
programowania z AI, także różne, że tak
powiem, tematy. Tutaj pas żółty jest
droższy, w nim też jest Perplex City Pro
na rok i też chociażby godzina
konsultacji. I mamy też czarny pas. To
jest roczny plan, czyli raz płacisz i
też ta cena jest o wiele tańsza, bo ona
chyba wychodzi z tego co pamiętam 10
miesięcy, czyli dwa miesiące oprócz tej
przeceny jest po prostu taniej. Także
też zapraszamy was, jeśli jesteście
zainteresowani. A to też jak wygląda
społeczność w środku. Mamy taką
społeczność na schoolu. Dzielimy się,
tak jak mówię, różnymi wątkami. Tu są
chociażby różne benchmarki. też już
tutaj trzy godziny temu była też moja
taka synteza tego, co ciekawego jest w
tym nowym modelu Opus 4.7. E, przeróżne
pytania od innych uczestników, też nasze
warsztaty i też to co ciekawe myślę
Classroom, czyli zakładka z przeróżnymi
miniursami, które przygotowujemy.
Mieliśmy ostatnio warsztat z Open Clow.
Tutaj pokazywaliśmy jak po kroku takiego
agenta uruchomić i to za nieduże
pieniądze, bo bo nawet w ramach takich
parunastu złotych już można było coś
takiego sobie wystartować na swoim
serwerze. Są też lokalne modele, czyli
jak się zabrać do tego z głową, czy to w
firmie, czy nawet prywatnie przetwarzać
przeróżne dane bez wycieku, tak, tego do
chmury, bo wtedy korzystamy z z modeli
na naszym komputerze. Są też fundamenty
A ja, czyli bardzo, bardzo takie
podstawy, chociaż też jest dużo takiej
usystematyzowania wiedzy, czym właściwie
są llmy, jakie są konkretne parametry,
jeśli chodzi o różne, o różne tutaj
ustawienia naszych lmów.
też wytłumaczenie jak pracować z
dokumentami, czym właściwie właśnie są
te LLMy. Także też tutaj w ramach takiej
społeczności przygotowujemy lekcje i też
tutaj co Krzyśka Krzyśkowi muszę oddać
to w ramach tych lokalnych modeli też
dał dużo serducha, bo przygotował
materiały łącznie tam z 40 parę minut,
które pokazują też jak robi taki setup
po prostu instalację u siebie na
komputerze, jak sobie to dokładnie
skonfigurować. Oczywiście też tutaj są
lekcje do tego też o małych modelach
językowych, także staramy się
przekazywać tą wiedzę w takim prosty,
przejrzysty sposób i też tak, żebyście
byli na bieżąco z tym, co się dzieje. Bo
ja nie ukrywam, jest to na pewno
wyciągające i też patrząc pod uwagę na
biorąc pod uwagę na to ile tych rzeczy
się dzieje w tak krótkim odstępie, no to
no to żeby być na bieżąco, no to
naprawdę trzeba by było po prostu
traktować to jako osobną robotę i nad
tym siedzieć i na bieżąco analizować, co
się dzieje w tym w tym internecie, bo
tego jest naprawdę dużo. Także jeśli
chodzi o to, materiały bonusowe już wam
też się pojawiły na mailu. Wysyłałem
linka oczywiście wyżej, także to też
macie i też zniżkę do naszej
społeczności wraz z opisem, co dokładnie
w niej jest. To też dostajecie na maila.
Ta zniżka zostaje do 17 kwietnia. Tu
jest licznik, czyli do za 27 godzin 32
minut tej zniżki nie będzie.
Dostawaliśmy maile, pamiętam, parę parę
tam minut, parę czasami godzinę po
północy z zapytaniem, czy można jeszcze
dołączyć. Niestety też chcemy być, że
tak powiem, fair z osobami, które które
dołączyły do nas w tym w tej okazji, w
tej ofercie, więc nie robimy, że tak
powiem, takich kart ulgowych, żeby kogoś
wpuszczać po tym konkretnym oknie. Jeśli
ktoś się załapie na tą lepszą cenę, to
no może po prostu dołączyć w tańszej
ofercie. Jeśli nie, no to po prostu
będzie musiał zapłacić 149 zł. To jest i
tak, uważam, bardzo dobra cena, jeśli
chodzi o te rzeczy, które znajdziecie w
środku. E, także to tyle ode mnie. Może
też Krzyśku powiesz coś yyy od siebie.
>> Jak w ogóle ty to oceniasz i co
ciekawego w ogóle robiliśmy w
społeczności. Jasne. Ja chciałbym tutaj
w ogóle zaznaczyć, że nieważne na jakim
etapie yyy jesteś rozwoju tutaj
sztucznej inteligencji, czy dopiero
zaczynasz, czy na przykład jesteś też
osobą taką bardziej techniczną i
wymagasz takich bardziej zaawansowanych
materiałów, w ramach społeczności
zagospodarowujemy zarówno obie oba
obszary, czyli osoby, które dopiero
wchodzą na w tą przygodę ze sztuczną
inteligencją, mogą sobie właśnie przejść
do materiałów klas roomie, gdzie obejrzą
sobie te fundamenty AI, z których
właśnie dowiedzą się w jaki sposób
efektywnie rozmawiać z tymi modelami AI.
Mogą też przejrzeć
warsztaty czy też porozmawiać, poodbijać
wiedzę z innymi osobami, które zawsze
tutaj chętnie pomogą, czy to zarówno my,
czy osoby wewnątrz społeczności. A też
takim dużym bonusem jest na pewno dostęp
do nas, bo my tam staramy się być bardzo
aktywni i staramy się odpisywać na
wszystkie rzeczy. Więc tutaj nawet nie
wiem Krzyśku, mógłbyś w międzyczasie
pokazać, zobaczyć, że jak są jakieś
pytania, my bardzo szybko reagujemy i
dajemy gotowe praktycznie rozwiązania do
wdrożenia
tutaj osobom. Tak więc jak tutaj
przefiltrujemy choćby po questions,
tu jest akurat właśnie podejście w jakiś
sposób z skillami, ale też
automatyzację. nowy film na YouTube na
przykład do toista już tam minąłeś to
Krzyśku i troszeczkę wyżej jeszcze jeden
wyżej o dokładnie więc jak tutaj
zobaczycie no my staramy się bardzo
szybko tutaj odpisywać i dawać konkretne
rady w jaki sposób to zrealizować tak
zadanie które jakaś osoba
>> jesteście zblokowani zastanawiacie się
jak je obejść i potrzebujecie że tak
powiem białkowej pomoc doradztwa to to
też w ramach takiej społeczności
oczywiście jesteśmy I służymy pomocą.
>> Dokładnie. No i tak jak widzicie
realizujemy co dwa tygodnie. Macie tutaj
na przykład warsztat z Robertem, który
prowadził OSPEC Driven Development,
czyli w jaki sposób może pokażę
warsztaty jakie mieliśmy w ogóle.
>> Tak, tak.
>> Tak. I warsztatów, które robiliśmy
wcześniej to też mamy warsztaty z
ekpetami. Już mieliśmy pięć takich
wydań. Zaraz będzie się szykować szóste
też stworzenia stron w takich nocodowych
narzędziach dla osób, które są
nietchniczne. Także budowanie stron to
jest na pewno yyy temat, który w ogóle
poruszyliśmy na starcie z Krzyśkiem. Yyy
i uważam, że to był naprawdę dobry
materiał godzinny, gdzie podzieliliśmy
się konkretnymi tipami to, jak stworzyć
stronę, która nie wygląda jak AI Slope.
Tutaj zresztą macie gdzieś tam malutki
spoiler tego, co tutaj poruszaliśmy
i też w ramach takich y w ramach takich
po prostu warsztatów robimy taką notatkę
podsumowującą, żebyście dokładnie
zobaczyli
co ciekawego poruszyliśmy, tak żebyście
mogli to szybko straw. To są czasami
warsztaty po półtorej godziny, także na
pewno takie notatki podsumowujące są po
prostu łatwiejsze do wybaczcie
strawienia. To na pewno to.
>> No i też staramy się tutaj pokrywać
wszelkie takie obszary, bo na przykład
warsztat numer 3 dotyczył bezpieczeństwa
pracy z modelami AI na produkcji, czyli
w jaki sposób walidować to, co wchodzi i
wychodzi z tego naszego modelu, aby nie
zrobić sobie krzywdy w firmie. Więc
tutaj mamy naprawdę taki szeroki
przekrój materiałów od takich osób,
które dopiero zaczynają swoją drogę aż
po takie mega zaawansowane rzeczy. No i
też warto zaznaczyć,
że cały czas staramy się tutaj rozwijać
te materiały. Czyli na przykład w
Classroomie, jeśli są jakieś lekcje,
choćby programowanie z AI, no to od
czasu do czasu wlatują tam jakieś nowe
lekcje
i staramy się je na bieżąco
aktualizować. No i też yyy wielką
wartością jest ta zakładka community,
gdzie dzielimy się y zarówno jakimiś
newsami, przemyśleniami, jak my
pracujemy, bo my też często zdradzamy
tajniki AA ninjas, czyli w jaki sposób
my podchodzimy do zarządzania zadaniami
czy kilkoma innymi elementami, które
wykorzystujemy w ramach naszego
warsztatu, czy to automatyzacji, czy
pracy z AI. Więc też można sporo się
dowiedzieć jak my pracujemy za kulisami
Aa ninjas.
Także
>> nie ukrywam, że ta praca się bardzo
zmienia. Z każdym miesiącem ta praca
potrafi ewoluować i i troszeczkę
zmieniać tą formę. Chociaż, że tak
powiem, fundamenty na pewno są stabilne,
no ale tutaj dużo rzeczy i takich
różnych rozwiązań wychodzi, że można tą
pracę jeszcze bardziej optymalizować,
jeśli chodzi o to.
Także tutaj zachęcamy was do dołączenia
do ninjas. A już tutaj widzę, że
pierwsze osoby nam zaufały i do nas
dołączyły, także wielkie dzięki.
>> Dziękujemy bardzo jeszcze raz
>> i myślę, że to będzie na pewno owocna,
że tak powiem, współpraca. A ja tylko
dodam od siebie, że tak naprawdę ten ten
to dołączenie jest bez ryzyka, a
mianowicie macie 14 dni, żeby tak
naprawdę się zapoznać z z tym co
oferujemy. I tak naprawdę jeśli do 14
dni stwierdzicie: "Okej, to nie jest dla
mnie, to mnie nie interesuje", to równie
dobrze możesz po prostu napisać nam
wiadomość, a my zwrócimy ci pełne
koszty. Tu oczywiście nie ma żadnych
ukrytych dodatkowych jakiś prowizji,
także po prostu jeśli zapłaciłeś 349 zł
albo 99 zł za pakiet, no to oddamy ci
pełną kwotę. Oczywiście pod warunkiem,
że napiszesz nam tą wiadomość i powiesz:
"No to nie jest dla mnie". Także, także
oczywiście może być tak, że stwierdzisz,
że po prostu to ci się nie przydaje albo
nie widzisz jak możesz to wykorzystać,
to w każdej chwili do tych 14 dni możesz
po prostu z tego zrezygnować. Także no
też to co gdzieś tam chcę zaznaczyć to
nie jest to w żaden sposób jakieś
ryzyko. Tak. A myślę, że po pierwszych,
że tak powiem, wykorzystaniach tego, co
zdobędziecie tam wiedzę, bo tam też były
chociażby informacje odnośnie
automatyzacji reklam, marketingu właśnie
skrapowania, wyciągania wiedzy, ofert
różnych czy też konkurencji, no to jest
na tyle tej wiedzy w tych warsztatach i
w materiałach, że tak naprawdę to się
powinno zwrócić wielokrotnie po
pierwszym miesiącu. Także tutaj to jest
taka gwarancja moja słowna, że tak
powiem. Oczywiście nie jest żadna
oferta, że tak powiem, finansowa. To nie
są, to nie są żadne gamblingi. Tutaj nie
mamy ruletki. Natomiast jeśli będziecie
chcieli naprawdę coś z tego wyciągnąć
dla siebie, no to myślę, że w ramach A
Ninjas na pewno to znajdziecie.
I co? Przechodzimy Krzyśku tutaj. Jak
już osoby pierwsze dołączają, nie
pierwsze, ale że tak powiem po tym
warsztacie, no bo już już tak powiem nie
prowadzimy tego tej społeczności od
teraz, to może przejdziemy do tych
pytań. które się pojawiały, a było ich
bardzo dużo.
>> Jasne, już tutaj przechodzimy sobie
spokojnie. M a tutaj dla was jeszcze
przypomnienie właśnie tutaj z tą zniżką,
że do 2359
do jutra, a my sobie teraz na spokojnie
przejdziemy przez te wszystkie
pytania, które się pojawiają.
Także jeśli macie jakieś pytania to
wciąż zachęcamy.
Ja już tutaj sobie przechodzę na sam
początek, bo dzisiaj no naprawdę sporo
pytań się pojawiło.
>> Tak dużo było. Widziałem no w trakcie.
>> Tak,
okej, już tutaj patrzę jakieś takie.
Okej, bo widzę tutaj też była jakaś taka
dyskusja o notebook elemie
i pewnie a pojawiły się też tam dalej
jakieś pytania o różnicę z notebook
elmem a obsydianem. Jakbyś tak Krzyśku,
nie wiem, miał powiedzieć
czy używać notebook Elma czy Obsidiana.
W jakim kierunku ty raczej wolałbyś
pójść?
Myślę, że notebook LM to jest jakaś też
narzędzie, jakaś warstwa, którą można
wykorzystać na pewno do syntezy, tak?
Czyli możemy wrzucić tam różne linki,
dokumenty i faktycznie możemy tą wiedzę
wyciągnąć. Natomiast to, co na pewno, to
co na pewno jest w kontekście notebooka
LM to to, że działamy trochę w
zamkniętym, no nie trochę, działamy w
zamkniętym narzędziu, to to znaczy nie
wiemy dokładnie co się dzieje pod
spodem, możemy się domyślać. Natomiast
to jest jakieś narzędzie, które
przygotował Google. Też są różne limity,
które są w ramach tego notebooka. Jak
mamy oczywiście konto pro, to mamy tutaj
więcej do działania. Jest to fajne
narzędzie na pewno. Natomiast ja bym
trochę nie patrzył na wybór to lub to, a
mianowicie nic nie stoi na przeszkodzie,
żeby takiego obsydiana zintegrować sobie
z notebookiem i pobierać od niego
właśnie te różne research, notatki. To
może działać równie dobrze jedno z
drugim.
Ja widzę przewagę Obsydiana w tym, że to
jest właśnie lokalne na waszym
urządzeniu, czyli wy nie potrzebujecie
dostępu do internetu, żeby te notatki
przeglądać. No GoogleM no to to jest
platforma, strona, na której musicie być
zalogowani, żeby przeglądać to w
chmurze, także też wymaga konta Google,
więc Obsydian jest o wiele lżejszy,
działa na tych plikach markdownych. No i
możemy je dokładnie jak chcemy
przerabiać, edytować. Mamy też ten
podgląd grafowy, pokazać jak te notatki
się ze sobą łączą. No i myślę, to co
jest takie najważniejsze, to co powinno
tu wybrzmieć, to jest właśnie prywatność
i 100% rozwiązanie lokalne, tak? Czyli
ty jesteś właścicielem swoich plików.
Jeśli obsydian kiedykolwiek przestałby
działać, no to twoje notatki i tak nadal
zostają jako pliki tekstowe, które
utworzysz w dowolnym innym programie.
też to co zaznaczam to też
personalizacja, czyli ogromna
społeczność, która tworzy tysiące
różnych wtyczek, pluginów, więc tego
obsydian jesteśmy bardzo yyy mocno w
stanie skustomizować na swoje potrzeby,
dostosować go. W przypadku Notebooka LM
no korzystamy z tego, co nam daje yyy po
prostu Google, tak więc no mamy pewne
ograniczenia jak to działa. Notebook
daje nam gotowe narzędzie, to jest
super. Natomiast wraz z właśnie
obsydianem jesteśmy w stanie to
workflow, ten swój przepływ tych notatek
dostosować do swoich potrzeb,
zintegrować go z różnymi narzędziami.
Notebook M to co powiedziałem może być
jedną z źródeł z których korzysta
Obsydian. Nie wiem Krzyśku jak ty na to
patrzysz,
>> ale to też jest ciekawy take.
Zupełnie się zgadzam z tym co
powiedziałeś. Natomiast ja też bym
rozwinął jeszcze tą część prywatności,
bo jeśli zależy nam na tej prywatności,
to nic nie stoi na przeszkodzie, aby
użyć lokalnych modeli. I ja też
podpinałem sobie pod cloud coda Bielika
7B Mitron i okazuje się, że świetnie
sobie radzi zarówno z syntezą tych
notatek, czy też odpowiadaniem na
pytania.
Więc pod względem takiej jakości nie
widać dużej różnicy względem właśnie
tych modeli Antropica.
Aczkolwiek na pewno jest to dużo
wolniejsze, ale wtedy mamy pełną
prywatność, a dla niektórych to też może
być kluczowe, zwłaszcza w firmach,
>> żeby też te nasze materiały nie
przychodziły, bo oczywiście trzeba też
można używać właśnie takich modeli jak
Gemina, jak Cloty z tymi naszymi
modelami, naszymi notatkami, ale wtedy
trzeba zadbać o m po prostu anomizację
tych danych, czyli musimy sobie
zamieniać te nasze dane wrażliwe na
jakieś takie zwane placeholdery, tak?
Czyli takie na przykład zamiast mieć
numer PESEL, to będziemy mieli na
przykład w takich nawiasach wąsowych
słowo PESEL, tak?
>> I dzięki temu też po prostu unikamy
wycieku tych naszych danych, ale też
trzeba o to umieć zadbać, żeby to
efektywnie przekształcać, tak? Te
notatki,
>> nie? No jasne, jasne pewnie. I to już
kwestia tego, co dokładnie przetwarzamy.
Ja akuratnie korzystam z Cloda, więc no
tak, mamy prywatność, mamy te notatki u
siebie, ale dalej, jeśli korzystamy z
jakiegoś modelu pod spodem, który jest
chmurowy, no to tak, to to nie jest może
pełna prywatność, ale to właśnie kwestia
tego, co tam dokładnie mamy. Ja akurat
nie korzystam z Cloda, bo tworzę sobie
takie Vty, gdzie syntetyzuję tą wiedzę i
też te moje notatki chociażby z Notion,
to są takie rzeczy, którymi mogę się
śmiało podzielić z zeajem i on może mu
im nadać drugie życie. Ale to co mówisz
Krzysiu to też jest fantastyczne. Jeśli
ktoś ma wystarczająco, że tak powiem,
zasobów na swoim komputerze, a teraz te
modele są coraz to te lokalne, coraz to
bardziej mądrzejsze, to też śmiało można
wykorzystać nawet to, co pokazałeś w tym
w tej lekcji właśnie na społeczności w
ramach lokalnych modeli do podpięcia
tego pod właśnie naszego obsydiana.
Także myślę, że to jest też świetne
zastosowanie.
Rozgadaliśmy się bardzo.
>> Mhm. Tak, mamy tutaj pytanie, czy będzie
nagranie. Tak, oczywiście będzie
dostępne.
Yyy, tak i od razu tak jak mówię też
materiały dodatkowe, tam też znajdzie
się link do YouTubea, zostały już
wysłane na waszego maila, także
będziecie mogli na spokojnie po po tym
warsztacie się z tym zapoznać, jeśli
jesteście zapisani na AI Ninjas. Tak.
>> A tutaj w ogóle Tomek pisze, że ostatnio
namówili mnie na Open Clow. Po dwóch
tygodniach zutylizowałem Homara.
Okej, chętnie też się dowiemy. Tak,
chętnie też się dowiemy,
co co było przyczyną właśnie utylizacji.
>> Nie, tak, Open Clow. Ja poruszaliśmy na
poprzednim warsztacie. Ja OpenClowa mam
też na swoim WhatsAppie zintegrowanym na
swoim serwerze VPS. To jest poprzedni
materiał, także też zapraszamy. A te
technologie ewoluują. I teraz dużo clot
clot sam w sobie wdraża takich rozwiązań
też podobnych do tego co oferuje
OpenClow. Natomiast dalej OpenClow to
jest projekt otwarty, także można go
dostosować do swoich potrzeb i nie
jesteśmy uzależnieni od żadnego
dostawcy. Także myślę, że to jest duży
plus jeśli chodzi o to rozwiązanie. Nie
wiem co dokładnie tutaj, że tak powiem,
Grzesiowi nie zadziałało. Co w sytuacji
kiedy notatek plików mamy już tyle, że
czytanie ich przez cloda pożera
większość tokenów. Czyli tutaj
rozmawiamy o zarządzaniu z większymi
takim.
>> Ja może pokażę tutaj ten mój diagram, bo
akurat
tutaj omawiałem właśnie co warto zrobić
dalej. No i właśnie jeśli dochodzimy do
momentu, kiedy słabo się skalują te
już rozwiązania oparte o cloud coda, bo
nie wiem, nie mieści się to w tym
kontekście, to o tym też w ogóle dość
mocno Andry Carpatti wspominał, że to
jest od 100 do 2000 notatek, w
zależności jakiego rodzaju
przechowujecie, jaki model używacie i
tak dalej, w końcu dojdziecie do tej
ściany. Hmm, dlatego też yyy Andry
Carpati, on ma takie podejście, że on
tworzy kilka Wiki i każde Wiki yyy
dotyczy konkretnego obszaru, tak? Czyli
na przykład ma Wiki związane z biznesem,
Wiki związane z programowaniem, Wiki
związane z czymś tam innym. To jest
jedna z opcji,
>> jak można rozwiązać ten problem. Ale
lepszym rozwiązaniem, które ja zacząłem
budować sobie już tutaj na boku, jest
właśnie yyy rozwinięcie tej koncepcji,
którą dzisiaj wam y zaprezentowaliśmy.
właśnie na przykład multimodalnego raga,
czyli taką naszą bazę wiedzy, którą
zamieniamy na te wektory, z którymi
później możemy sobie za pomocą tych
modeli rozmawiać
i dzięki temu
jesteśmy w stanie przetwarzać już no o
wiele wiele rzędów więcej tych notatek
niż za pomocą takiego samego cloud coda,
który w pewnym momencie jak dojdziemy do
odpowiedniej skali zacznie już się gubić
w tych naszych notatkach, bo choćby
załadowanie tego pliku index, tak, który
mamy, czy pliku z logami, on już będzie
na tyle duży, że on będzie zapełniał
praktycznie, nie wiem, w całości ten
nasz kontekst. No i wtedy no rozmowa z
tymi notatkami
no nie będzie w ogóle efektywna. Dlatego
będzie trzeba sięgać po takie
rozwiązania właśnie jak rak.
Nie wiem czy ty się akurat tutaj Krzyśku
zgodzisz z tą tezą czy jednak poszedłbyś
w innym kierunku czyli dwie dwie opcje.
Albo tworzenie osobnych Wiki, albo
rozwijania jako jedno źródło wiedzy z
dodatkowym ragiem.
Nie no to akuratnie to jak ja na
przykład pokazałem tego Obsidiana, ten
Obsidian Research to było typowo takie
wiki skupione na jednej domenie, jednym
temacie, czyli research obsydiana i to
działa bardzo fajnie. Jeśli chcemy, bo
też takie pytanie się pojawiło, jak
właśnie zarządzać, jeśli mamy parę wtów,
jak, czy one mogą się wymieniać
informacjami i tak dalej, to ja w takim
podejściu polecam zbudow, jeśli mamy
jakąś wiedzę, którą chcemy dziedziczyć
między różnymi wtami, to czemu nie
zrobić 1 Vta, który będzie właśnie w
takiej w takim schemacie para, takiej
metody para, które służy do tego, żeby
na przykład możemy mieć różne obszary,
tak, naszych projektów, które się ze
sobą łączą. Na przykład tak jak my mamy
AI Ninjas, Krzyśku, działamy nad AI
Ninjas. Ja działam też nad swoimi
projektami. Mam swojego YouTubea, gdzie
też dzielę się wiedzą ze o sztucznej
inteligencji i dużo tematów, że tak
powiem, ze sobą są połączone. Mam
newsletter detective, tak samo o
sztucznej inteligencji, więc ja lubię
mieć też swój projekt, gdzie łączę parę
tematów i to jest również okej.
Natomiast jeśli chodzi o skalowanie, no
to no to myślę, że to też trzeba dobrze
zastanowić się nad strukturą w ogóle
naszego obsydiana. I też myślę, że to
jest kwestia tego takiego mądrego
zarządzania tymi notatkami i
aktualizowania tej bieżącej wiedzy, bo
też oprócz takiej higienizacji, tego
lintowania, też warto się zastanowić,
czy ta wiedza, którą mamy gdzieś tam
wrzuconą, którą już nie aktualizujemy od
nie wiem od paru, od paru tygodni,
miesięcy, czy ona powinna być w jakimś
stopniu zarchiwizowana, jeśli to już nie
jest nieaktualne. Tak więc więc tutaj
trzeba też mądrze do tego podchodzić,
nie tylko dorzucać, dorzucać, dorzucać,
ale też mądrze, że tak powiem, tym
zarządzać i też czasami poczyścić pewne
rzeczy, które są już nieaktualne albo je
zarchiwizować, żeby nie brać ich pod
uwagę na przykład w w querowaniu. Tak
myślę, że na tyle ta ta baza grafowa
właśnie te połączenia grafowe dają tą
przewagę, że CL jest w stanie bardzo
szybko przyłączyć fakty po prostu i
łączyć tą wiedzę z różnych notatek,
czego jakby nie miał, no to musiałby sam
sobie po prostu syntetyzować i szukać
tych informacji jak ze sobą połączyć
konkretne fragmenty. Tutaj po tym
połączeniu grafowym on od razu też
widzi, więc myślę, że to jest pewne
jakieś ułatwienie i oszczędność tokenów,
jeśli korzystamy z Obsidian CLI, bo też
z Obsydiana możemy korzystać z linii
comand, co jest świetne do integracji z
właśnie agentami. Nie wiem o potencjałm,
>> ale prawdziwy potencjał według mnie y
ukazuje się, kiedy połączy, zrobimy
takie hybrydowe rozwiązanie, kiedy
połączymy właśnie tą bazę grafową, którą
mamy w obsydianie z bazą wektorową,
czyli korzystamy z obu, aby uzyskać
informacje i wtedy to naprawdę,
uwierzcie mi, że
skuteczność rozmowy z tymi notatkami no
rośnie no dyetralnie.
A tutaj Krzyśku wspominałeś o tych kilku
voltach, nie? Że ktoś tutaj wychodził od
takiego pytania, że ma kilka voltów. No
i w sumie jest na to rozwiązanie jak
efektywnie korzystać, nawet mając w
kilku voltach, bo mamy coś takie jak
Obsidian CLI, który pozwala nam się
łączyć do różnych voltów, więc możemy
sobie w projekcie na przykład jakimś tam
clot codzie mieć plik, który opisuje, że
hej, w tym wolcie trzymam to, w tym
trzymam to, w tym to. Możemy też na
poziomie publiczny prywatny Volt to
realizować, tak? I do prywatnych na
przykład on nie będzie miał dostępu,
tylko do publicznych, więc za pomocą
Obsidian CLI, mając kilka voltów, możemy
z innego projektu się dobierać nawet do
pięciu różnych Vtów. A te, które są
oznaczone jako prywatne, no to sorry,
ale nie pozwolimy tam ci wjechać, nie?
Więc też możemy sobie to ograniczać na
sposób taki, że w voltach publicznych
trzymamy
>> notatki, które y możemy upublicznić
nawet każdemu, tak? Bo to są jakieś, nie
wiem, nasze notatki związane z blogami,
artykułami, newsami i tym podobnymi
rzeczami, których wyciek niczym nam tak
naprawdę nie grozi i one mogą być sobie
nawet publicznie w internecie, ale
możemy też mieć notatki prywatne, na
przykład związane z naszą firmą, które
będą trzymane w voltach, które są
oznaczone jako private i dzięki temu też
zapewniamy, że na przykład taki cloud
code za pomocą tego obsidiana na kilku
oczywiście mechanizmach, nie możemy
tylko ufać temu Obsidian CL i Cloudowi,
że on tam nie wejdzie do prywatnego i
jesteśmy w stanie to realizować.
>> Dobra, kolejne pytanie. Może tyko
powiem, że też teraz eksploruję takie
takie repozytoria i różne koncepcje
jeśli chodzi o obsydiana, mianowicie też
różnego podejścia do tego wyszukiwania,
czyli do pobierania tej informacji. No
bo mamy ten taki native search, czyli po
prostu, że szukamy sobie chociażby z tym
Obsidancy Lip, to co powiedziałeś, mamy
też ten gra viiew, natomiast też można
pójść o krok dalej i robić jakiegoś na
przykład fuzji searcha. Możemy też
zrobić właśnie jakieś wyszukiwanie
semantyczne. Można po prostu to w różne,
>> tak? Także oczywiście tu są to co
powiedziałeś wymagane embedingi, ale też
możemy pójść o krok dalej i coś takiego
zrobić. Także to jest, myślę, że tak
naprawdę też ciekawe rozwinięcie i
myślę, że też w jakimś wątku na
społeczności to poruszę, jak po prostu
będę już miał, że tak powiem,
wypracowaną jakąś swoją metodykę, jeśli
chodzi o to, bo to jest ciekawy temat.
Znaczy, no chyby nowe rozwiązanie według
mnie, gdzie mamy bazę tą grafową plus
bazę wektorową, no
bardzo mocno tutaj
zwiększa tą skuteczność i możemy
przeować nawet miliony tych naszych
notatek.
>> Możesz pokazać mój ekran na chwileczkę
jeszcze, bo właśnie jedną rzecz tylko
bym pokazał jeszcze. Możesz oczywiście
kontynuować. Ja tylko chciałem pokazać,
że mam tutaj te oczywiście row właśnie
te surowe pliki, różne notatki, ale
później też w syntezie, co ważne mam też
przeróżne tagi, mam też skąd jakie są
source właśnie ten poziom confidence,
czyli też różne takie tagi, które
pozwalają później llmowi, naszemu AIowi
querować po tych notatzkach. Czyli on je
nie nie szuka tylko po samym, że tak
powiem, jakimś słowie, jakimś znaczeniu,
tylko też jest w stanie wyszukać po
konkretnym, e, na przykład sprawdzić,
kiedy te notatki, na ile one są
aktualne, zobaczyć po tgach, może coś po
tagach już znajdzie ciekawego. Także też
ten poziom y zaufania do tych notatek,
czyli im wyższy, to znaczy, że jest
poparty większą ilością źródeł. To też
są ciekawe sposoby jak można, że tak
powiem to wyszukiwanie robić jeszcze
mądrzejsze, inteligentniejsze przez
właśnie różne metadane, które dodajemy y
z poziomu właśnie tutaj atrybutów do
danych notatek. I to też jest w stanie
wam prowadzić lm i też jako taki lm azaj
judge po prostu oceniać wam, które te
notatki są warte, a które są na przykład
marketingowe. Ja ci powiem tylko Krzyśku
jeszcze jedną wstawkę. wrzuciłem mu
materiał, jeden ciekawy blog, który
miałem, który nie przeczytałem tak
naprawdę i stwierdziłem, brzmi ciekawy
jakiś wstęp, wrzucę i zobaczę, co mi
powie mój obsydian, czy może już takie
wiadomości mam. I on mi powiedział
Claud, że po prostu to jest jakaś
marketingowa papka. I faktycznie pod tym
blogiem była jakaś firma, która
sprzedawała swoje rozwiązanie i tam
Obsydiana było mało samego w sobie, ale
przez to dostałem informację od Cloda,
czy na pewno chcę to dodać i wtedy się
zawahałem i stwierdziłem faktycznie nie
będę dodawać sobie jakiegoś
marketingowego, że tak powiem, jakieś
paplaniny do mojej bazy, bo to będzie
zaśmiecanie jej. Tak, także to jest też
o tyle fajne, że ja na przykład gdzieś
tam na szybko wrzucając te dane nie
wyłapałbym tego, a my możemy sobie to
skonfigurować z poziomu cloda, tak że on
będzie w stanie zweryfikować te źródła i
zobaczyć co tam dokładnie jest. Tak,
możemy w ogóle sobie, ja to jeszcze
rozwinę tą twoją koncepcję, możemy sobie
stworzyć prosty filtr. Możemy w jakimś
pliku markdownym, czy nawet w Excelu,
gdziekolwiek mieć
przygotowane takie filtry, jakie treści
nas interesują, bo załóżmy, nie wiem,
dodaje, mamy jakieś RS Fit, tak, który z
automatu, nie wiem, raz dziennie dodaje
x notatek. No i na przykład dodajemy
sobie notatki związane z finansami, tak?
tak szeroko powiedzmy finansami. No i
pojawiają się tam na przykład notatki
związane z Forexem. Na przykład my nie
jesteśmy zainteresowani Forexem, bo nas
interesuje nie wiem jakieś oszczędzanie,
jakieś wiesz, jakieś takie pasywne
inwestowanie w ETFY i tak dalej, więc
Forex nie jest dla nas. Więc możemy
sobie albo w tej tabelce na Excelu, albo
nawet w pliku markdowym wpisać w ramach
filtrów na blackliście Forex. No i teraz
jeśli my pobieramy jakieś materiały
związane z Forexem automatycznie tutaj
nasza baza wiedzy tego nie będzie
dodawać, bo to nas nie interesuje, więc
możemy sobie tworzyć filtry zgodnie z
naszymi zastosowaniami, tak? Yyy, z
naszymi upodobaniami, że tego typu
treści chcemy, tego nie.
>> Tak. Mhm.
>> No i no i dzięki temu możemy też mieć
notatki tylko, które nas interesują. Na
przykład nie wiem, z AI interesują mnie
na przykład, nie wiem, tylko rzeczy
związane z ekosystemem Googlea. Więc
jeśli będę chciał coś wrzucić z
antropikiem, no to Vol się zapyta: "Ej,
stary, na pewno ty chcesz to wrzucić, bo
przecież
powiedziałeś, że te wiadomości o
antropiku cię nie interesują, więc
możemy se dowolnie tworzyć takie filtry
w bardzo prosty sposób".
Musimy przyspieszyć Krzyśku, bo za
musimy przyspieszyć
pytań. Kolejne pytanie, które dotyczy
czy do tych notatek będę miał raz dostęp
na telefonie. Jeśli nie, to bez sensu.
Jak najbardziej możesz mieć i na to jest
kilka różnych sposobów. Jeśli nie chcesz
tego mieć publicznie dostępne, no to
możesz mieć to całkowicie lokalnie
zamknięte swojej sieci i wykorzystać
genialne narzędzie, z którego ja
korzystam od dawien dawna, czyli
Syncfing, czyli taki open sourceowy
projekt darmowy, który sobie
uruchamiacie na swoim komputerze i on
synchronizuje notatki w ramach waszej
sieci lokalnej, czyli masz, musisz
oczywiście być połączony do tego samego
Wi-Fi, na przykład z laptopem i z
telefonem i wtedy synchronizują się
notatki między tymi wszystkimi źródłami.
Kolejną rzeczą, jeśli chcecie mieć to
przechowywane już publicznie dostęp, na
przykład można wykorzystać GitHuba, tak?
Dzięki któremu
>> właśnie
>> któremu zyskujemy też jeszcze
wiele dobrodziejstw, które przynosi nam
git. Oczywiście tutaj nie chciałbym już
się jakoś rozwodzić, bo chcemy tutaj
przyspieszyć.
Natomiast kolejną rzeczą,
>> kolejną rzeczą jest na przykład
wrzucenie jakiegoś VPSa, nie?
albo na VPSie, czyli na swoim serwerze,
co nie? Tak jak pokazywaliśmy na
mikrusie poprzednio. Ja akuratnie to, co
chciałem powiedzieć, to też gdzieś tam w
ramach społeczności na dniach
popublikuję moją synchronizację, bo
tutaj też widziałem dużo komentarzy jak
to dodać na przykład na telefon. To co
Krzyśku mówisz też jest fajne, ale ja na
przykład właśnie robię przez KitHua i
taki projekt mi się automatycznie przez
pluginy aktualizuje, więc ja nie muszę
tego robić nawet ręcznie, nie muszę, że
tak powiem, aktualizować tego projektu.
on sam po prostu wrzuca zmiany na mojego
GitHuauba. Ja mogę później taki projekt
odpalić z poziomu telefonu. Nawet jeśli
ktoś nie ma specjalnych aplikacji do
tego, to równie dobrze może sobie takie
takie repozytorium podpiąć pod cloda z
poziomu asystenta webowego z telefonu i
też czy tam z aplikacji i też dodawać
jakieś zmiany. Także to jest na pewno
wygodne i proste.
>> No i no i żeby też to wybrzmiało. Na
przykład taki Synf, jeśli jest
wystawiony na świat, to z dowolnego
miejsca też się same synchronizują. On
po prostu śledzi foldery, które mu
mówicie, a dajecie mu całego volta i
wtedy cokolwiek się doda na wolcie,
macie praktycznie real time
odzwierciedlone na innych urządzeniach,
które po prostu są wpięte, tak do
śledzenia tego Volta. Więc wrzucam na
telefonie i od razu widzę na komputerze.
Dobra, lecimy dalej.
Dobra, tak patrzę tutaj jeszcze bąd
jakieś dyskusje między
tak konkretne pytanie tam widziałem, że
ludzie Q dwukropek robili, tak fajnie
oznaczali, widzę, że się taka konwencja
wyrobiła. To mi się bardzo podobało,
także możesz takie Q specjalnie też
powrzucać, bo bo myślę, że to też
może no to są konkretne pytania, na
pewno łatwo to odpiltować.
>> Okej. m czy te wiązania same się budują,
czy trzeba je jakoś magicznie zrobić. No
i właśnie tutaj za tą całą magię
odpowiada model pod spodem. Tak.
I to jest piękne w tym wszystkim.
Właśnie o to chodzi, żeby, znaczy ja
rozumiem, że ta cała koncepcja polega na
tym, żeby ręcznie tym wszystkim nie
zarządzać, nie pochłaniać się na
łączeniu tych notatek, ale pozwolić
lmowi, czyli naszemu modelu, modelowi
samemu właśnie ułączyć te kropki na
bazie tego, co już mamy. Także to, co
pokazywałem ja, to, co pokazywał
Krzysiek, ta baza się aktualizuje sama,
czyli ty nie musisz ręcznie wchodzić,
wrzucać notatki, robić podsumowania tej
notatki i następnie łączyć je z innymi
notatkami. Dla mnie jako osoby, która
jest, że tak powiem, nadreaktywna,
byłoby to za długie i ten proces by
trwał na tyle długo, żebym nie zrobił go
poprawnie. A teraz z klonem mogę sobie
to zautomatyzować. Oczywiście też warto
zweryfikować jakie połączenia powstają,
ale to możemy już później, że tak
powiem, wejść w tą notatkę i zobaczyć co
tam dokładnie jest. Także możemy to
później zweryfikować i też ewentualnie
poprawić. To jest akurat nieproste.
>> Kolejne pytanie. Czy mogę mieć jedną
stronę z linkami w katalogu row? Czy
każdy link musi być osobną notatką? No i
odpowiedź jest następująca.
Tworząc taki second brain czy wiki
personalizujesz pod siebie. Jak tobie
jest wygodnie pracować, tak to
realizujesz. A dla modelu wyciągnięcie
nawet 100 linków z jednego pliku
markdowego czy mieć 100 osobnych plików
to jest żadna różnica. Kwestia
zdefiniowania zasad, w jaki sposób
pracujesz.
>> Tak. Tak. Tutaj mamy dowolność.
>> Jak generujesz logi Obsydiana? Znów ta
cała magia dzieje się właśnie za pomocą
modelu. To wszystko jest zdefiniowane
zazwyczaj albo na poziomie jakichś
skillsów, albo pliku clot MD czy agents
MD. Tak. I tutaj opisujemy właśnie te
wszystkie zasady. w jaki sposób on
będzie generował te logi, w jaki sposób
będziemy dostarczać te notatki do tego
row, czy w jaki sposób on te wiki będzie
generował. Oczywiście my przestawiliśmy
jedną koncepcję, tak, Karpatieego, ale
nie znaczy, że ona jest jedyna słuszna.
Może warto wziąć tak jak Krzysiek i ją
dostosować pod siebie albo pójść w takim
kierunku jak ja, gdzie ja teraz buduję
w całkiem innej koncepcji
swój second, gdzie też inspiruję się
choćby takimi projektami jak Open Clow i
kilkoma innymi, z których wyciągam
ciekawostki i realizuję tutaj swój
second brain, który jest mega
zautomatyzowany.
>> Tak. I nawet chyba nie wiem czy w tym
templatecie, który wrzuciliśmy w ramach
maila i też społeczności
podzieliliśmy się właśnie tym szablonem
jak tworzyć takiego przykładowego Volta
takiego jak jakiego ja pokazałem to też
tam nawet definiowałem, określałem takie
reguły do do robienia logowania, więc
można też śmiało sobie podpatrzeć i
wziąć coś dla siebie. To jest na pewno
ciekawe. A także to tylko jeszcze tak
ode mnie dodając, to robi wszystko klot.
Dokładnie.
Graf rak.
>> Okej. Kolej
ten graf, który pokazałeś przed chwilą,
to był graf rak, czy po prostu jakaś
baza wiedzy na grafie? Prawdopodobnie to
było odniesienie do tego, co pokazałeś w
obsydianie. Tak. Obsydian. Tak, tak,
tak.
>> To jest obsydianowy graf pokazujący
połączenia między notatkami.
>> Tak. Tak. To są właśnie te linki, które
się znajdują po różnych notatkach, które
linkują do innych notatek. Stąd powstaje
taki ładny yyy graf.
Tutaj mieliśmy pytanie, jakie są, jakie
skille są potrzebne w clot, aby tak
fajnie to działało.
Teraz ciężko nam się odnieść po tak
długim czasie, więc jeśli jesteś z nami
jeszcze, Nexor, to chętnie m odpowiemy
na te twoje pytania, jakbyś doprecyzował
o co o co tam dokładnie dopytywałeś.
Znaczy rozumiem, że w tym obsydianie
jakie skille wykorzystujemy, żeby on tak
sprytnie, że tak powiem, działał. I ja
od siebie powiem, że sam Clot w sobie
bardzo dobrze radzi sobie z tą konwencją
Obsydiana. Nie potrzebuje tutaj dużo,
żeby się po nim poruszać. Oczywiście
możemy włączyć Obsidian CLI. On też
sobie może sam później poprzez helpa,
czyli taką komendę sprawdzić jakie ma
komendy w ramach Obsydiana. Natomiast są
też skille, które są publiczne na
GitHubie. Ludzie dzielą się takimi
gotowymi umiejętnościami, które też, że
tak powiem, szczegółowo definiują jak
się poruszać po takim po takich Voltach,
jak robić notatki. E, także to też chyba
w tych materiałach dodatkowych
projekt wrzuciłem Kipano Skills, Kipano
Obsidian Skills. Polecam sobie też
sprawdzić na mailu będziecie to mieli.
Tam są właśnie skille odnośnie tego, jak
tworzyć takie dokumenty markdown, jak
tworzyć bazy, tak, czyli te widoki takie
bazowe w Obsydianie, jak robić Jason
Canvas, jak się poruszać po CLI. Także
myślę, że to też są fajne, gotowe
umiejętności, które możecie później
dostosować do siebie, ale one nie są
wymogiem. To żeby było jasne, to nie
jest wymóg.
>> I warto dodać, warto dodać, że to są yyy
skille bezpośrednio od twórcy Obsydiana.
>> Dokładnie tak.
No i tutaj w sumie jest analogiczne
pytanie o te skillsy.
Zresztą tak jak ja pokazywałem u siebie
ten ingestne rzeczy to są po prostu
skillsy, które definiują w jaki sposób
on ma dokonywać tej kompilacji, tej
wiedzy. Więc ja też mam customowe
skillsy czy do tasków, które dzisiaj
pokazywałem.
Dlatego warto
tworzyć rozwiązanie, które jest
spersonalizowane pod nas. to co
potrzebujemy. Po prostu o to yyy
rozszerzyć ten nasz obsidian.
Ja tu tylko wyskoczę jeszcze szybko, bo
widzę, że Nexor odpowiedział tylko, że
doprecyzowanie chodzi clot yyy chodzi
clotzy dodatkowe skills instalowaliście
do obsydiana, aby ładnie szedł w proces.
To już powiedzieliśmy, czyli możesz
zacząć naprawdę z bazowym projektem
takim jak ja pokazałem i nie musisz
nawet mieć dodatkowy skill i on sobie i
tak dobrze z tym poradzi. Natomiast
jeśli dodasz skillsy, to na pewno będzie
taki nice to have dodatek, żeby
usystematyzować tą wiedzę, jak on ma
pracować z tymi twoimi notatkami
obsydianowymi. Myślę, że to nie
zaszkodzi, a może pomóc.
Dobra,
>> Katarzyna tutaj napisała, że zbudowała
swój secondin, ale nie z obsydianem. M,
oczywiście to nie jest jedyna słuszna
droga, aby budować second wykorzystaniem
obsydiana. Zresztą ja sam obsidiana
wykorzystuję tylko po to, żeby dostać
ten graf plus wikilinks.
Tak. A jako frontend ja wykorzystuję
po prostu antygravity. Tak, ja nie
wychodziłem z antygravity, gdzie
Krzysiek pokazał całkiem inne podejście,
gdzie on siedzi wyłącznie w tym
obsydianie, gdzie też sobie uruchamia
terminal i tak dalej.
Tak, bo to terminal, jeśli ktoś by
chciał uruchomić w ogóle z poziomu
obsydiana, to jest wtyczka, ona się
nazywa po prostu terminal dosłownie.
Także to, co ja pokazywałem, że miałem
takiego po prostu na pośrodku terminal,
to właśnie spowodowany tą wtyczką. Także
można sobie też to tak ustawić, żebyśmy
mieli w ramach tej aplikacji po prostu
dostęp do cloda.
No dobra, co tam jeszcze ciekawego?
Mamy
tutaj jest pytanie do ciebie Krzyśku.
Jak przeglądasz i dodajesz notatki z
telefonu?
>> To się już pojawiło, czyli po prostu
jestem w stanie sobie go zsynchronizować
po GitHubie. A i mam tą wtyczkę do Gita.
To też wrzuciłem w ramach materiałów
bonusowych. Jest to wtyczka Git. ona
pozwala mi zapisywać te notatki do
Githua, a później jak już mamy GitHub to
wystarczy jakie jakakolwiek aplikacja do
zarządzania repozytorium czy też po
prostu są też takie aplikacje, które
nadbudowywują, że tak powiem yyy nawet
musiałbym sobie przypomnieć, bo jest
teraz taka nowa aplikacja, którą
sprawdzałem dzisiaj, to się też podzielę
jak może gdzieś tam, że tak powiem, może
w mailu jakimś podrzucę albo w tych
materiałach bonusowych, która
wykorzystuje dosłownie tego GitHua do
integracji z GitHubem tworzy nam po
prostu taki no właśnie takiego obsydiana
w naszym telefonie. Natomiast można to
po prostu zrobić poprzez GitHuba. Ja tak
robię, że sobie łączę się z tym
projektem na telefonie nawet z poziomu
clot coda. Najprościej, czyli wrzucam w
zakładkę code, tam łączę się z moim
GitHubowym projektem i mam już do niego
dostęp i mogę z nim normalnie naturalnie
pisać. Także mogę wyciągać wiedzę, mogę
dodawać nowe rzeczy. Także to jest tak
bardzo, że tak powiem, banalnie
wytłumaczone. Można to wykorzystać w
clodzie. przeglądarkowym, ale również i
no tak jak mówię, można sobie pobrać
GitHuba i też wprowadzać jakieś zmiany z
poziomu telefonu przez inne aplikacje.
To jest już dowolnie, jak sobie to
ustalimy.
I tu kolejne pytanie. Czy masz własny
workfall do przetwarzania słabej jakości
źródeł? Mam sporo luźnych, niskiej
jakości notatek w Apple Notes. Nie
chciałbym zaśmęcać nimi row, zanim
zostaną wstępnie uporządkowane. Właśnie
po to jest ten row. Tam wrzucamy surowe,
nieuporządkowane notatki i właśnie
prchodzimy,
>> tak? I właśnie przechodzimy później
przez proces kompilacji za pomocą LLMA,
który nam już uporządkowuje, tak? Tworzy
syntezę, tworzy cały ten wyciąga z nich
koncepty, opisuje każdy koncept i tak
dalej. Więc wtedy dostajemy
uporządkowaną. Więc row to jest idealne
miejsce, aby wrzucać
jak to nazwałeś, słabej jakości źródła.
>> Do tego to służy. Dokładnie.
>> Kolejne pytanie. A jak jest z łączeniem,
dzieleniem wiedzy na różne obszary?
Każdy potrzebuje innej wiedzy. Cały
drugi mózg. Dokładnie. Już o tym
rozmawialiśmy. Albo rozbijasz to na
osobne wiki, albo tworzysz jedną
bazę wiedzy, ale w pewnym momencie
będziesz musiał rozszerzyć Oraga. Więc
zachęcamy tutaj też do powrotu y kilka
minut wstecz, gdzie o tym przez kilka
minut szerzej opowiadaliśmy.
Dobra, szukam teraz kolejnych pytań.
Okej. Czy będzie pokazane jak zrobić
sobie wszechstronny dostęp jak ty masz
na telefonie i nie tylko?
Tak myślę, że ogólnie większy setup
taki, że tak powiem, to co pokazaliśmy w
ramach materiałów bonusowych i też tego
co pokazujemy w ramach w ramach tego
warsztatu, no to na pewno taki no taki
pogląd na to z góry z tego powodu, że
nie jesteśmy w stanie wszystkiego
szczegółowo pokazać w ramach takiego
webinaru, warsztatu półtoragodzinnego.
Natomiast myślę, że też więcej będę mógł
zdradzić w ramach po prostu naszych
naszego community, gdzie już będziemy
mogli po prostu rozłożyć to na na
pierwsze, że tak powiem, na cząstki
pierwsze. I nawet nie myślę Krzyśku nad
tym, czy czy nie zrobimy tak, że nawet
zrobimy w ramach community po prostu
taki warsztat, gdzie sobie pokażemy te
konkretne nasze rozwiązania i skupimy
się na jakichś konkretnych
zastosowaniach, czy to właśnie tej
integracji pomiędzy różnymi
urządzeniami. To też mogę pokazać wtedy
już spokojnie przez godzinkę, jak można
z tym zarządzać z różnych po prostu
miejsc, tak żeby to ten obsydian nie był
tylko z poziomu komputera, ale wynieść
go właśnie też na inne na inne
urządzenia. No bo no o to w tym
wszystkim chodzi, żeby łatwo z tym
komunikować się z różnego miejsca, czy
jesteśmy w domu, czy jesteśmy poza nim.
Myślę, że to jest bardzo ważne.
>> Mhm. Znaczy warsztaty, które tutaj
realizujemy na YouTubie, to jest tak
naprawdę,
aby was zaciekawić, pokazać, sprzedać
wam konkretną koncepcję,
jak z tym można sobie pracować, trochę
przemycić teorii na ten temat i jak
ruszyć w ogóle z takim tematem.
Natomiast aby pokazać krok po kroku jak
zbudować coś takiego, jak porobić te
wszystkie integracje, jak wynieść to do
telefonu i innych rzeczy, to każdy z
tych elementów, który wymieniłem, to
jest przynajmniej warsztat na kolejną
godzinę, więc z tego moglibyśmy równie
dobrze zrobić kilkugodzinny warsztat,
jak stworzyć taki naprawdę
zautomatyzowany,
synchronizujący się między różnymi
urządzeniami
system do zarządzania wiedzą, więc no
ciężko jest po prostu pogodzić
to ile pokazać na takim warsztacie, żeby
zainspirować te osoby, bo jednak
budowanie krok po kroku to jest kilka
godzin tak naprawdę, żeby pokazać taki
cały proces.
>> Dlatego też dajemy w ramach Tak, dlatego
też to, co daliśmy w ramach materiałów
bonusowych, to macie gotowy szablon, z
którym możecie ruszyć już dzisiaj. Także
tutaj możecie go sobie pobrać totalnie
za darmo, zacząć z nim działać i
zobaczyć na ile wam to się przydaje
takim pierwszym od takiego właśnie, że
tak powiem, templateu, gdzie macie już
pewne szlaki przetarte. A jeśli
jesteście ciekawi dalej zgłębiania tego
tematu i wchodzenia jeszcze głębiej w
tego obsydiana i jego wykorzystania, no
to tu to już mówię, tu trzeba by było,
że tak powiem, jeszcze osobny materiał z
tego robić, no bo jest tego jest dużo
konceptów, tak? Są Zelkasteny, są
metodyki para, no właśnie jest chociażby
LLM Karpati, tak? Wiki, lm wiki
bardziej, tak? To jest bardzo dużo
konceptów w jaki sposób można tego
obsydiana rozwijać. Możecie go rozwijać
jako takiego asystenta, który ma wiedzę
o waszych różnych projektach, różnych
zadaniach, jeśli chodzi na na co dzień.
Tak, możecie sobie robić journal, czyli
notatki, dziennik w ogóle jakiś taki
codzienny, tak? Także bardzo dużo
koncepcji, które możecie robić od
rozwoju osobistego, poprzez budowanie
jakiejś wiedzy firmowej, poprzez jakieś
takie własne research, projekty, y, z
którymi chcecie właśnie w ramach takiego
Volta się podzielić. Także jest tego
bardzo, ale to bardzo dużo.
>> Mateo też zachęcamy tutaj do dołączenia
do społeczności, bo zawsze każdy temat,
który bierzemy tutaj na darmowy
warsztat, rozbijamy
głębiej w ramach społeczności i
pokazujemy właśnie jak krok po kroku
takie rzeczy sobie skonfigurować.
Kolejnym pytaniem, czy ktoś próbował to
wdrożyć w MŚP lub w organizacji dla
jednego konkretnego działu?
Szczerze mówiąc, no my tutaj z Krzyśkiem
już takie rozwiązanie sobie budujemy.
Wczoraj by
>> można powiedzieć, bo dla swoich firmy,
>> no ale o to chodzi, żeby zacząć od
siebie.
>> Tak, ja też buduję dla swoich
działalności
też takie swoje bazy wiedzy. Yyy, co
ciekawe, wczoraj też byłem na meetupie,
gdzie Kuba Masztalski, więc jak nas
słucha, to go serdecznie pozdrawiamy,
gdzie też właśnie opowiadał o tym, jak
on dla swojej firmy oraz jako usługę
świadczy też taką rzecz dla MŚP, gdzie
buduje właśnie takie secondy, gdzie też
pokazywał właśnie taką zmodyfikowaną
koncepcję Carpatiego, więc jak
najbardziej, jak najbardziej tego typu
rzeczy
się realizuje. Aczkolwiek tutaj też
trzeba mieć na uwadze, że momentami
niektóre rzeczy będą musiały być
zrobione, zadbana ta prywatność, więc
albo anomalizacja danych, albo
przetwarzanie też na lokalnych modelach,
więc to trzeba mieć na uwadze.
Okej, kolejne pytanie.
Inkes komenda to jest Klaudiuszowa. Czy
dogrywa się ją i wygrywa skille? Wgrywa
skille. To jest przeze mnie stworzony
skill, który dokładnie opisuje zgodnie z
konceptem Karpatiego w jaki sposób
przygotować tą kompilację wiedzy przez
LLMA.
>> Może Krzyku też to wrzucisz w ramach
społeczności. To też myślę, że ciekawa
będzie rzecz.
>> Tak, tak, tak. Właśnie tego typu skille
i tak dalej my się dzielimy teraz tutaj
na społeczności, więc pewnie w
najbliższym czasie będziemy to wszystko
udostępniać
członkom, którzy są.
Z kolejnego pytania sprawdziliście po
update aplikacji The SW Clot pojawiła
się zakładka additional features daily
included routine runs. To dość istotne,
jeśli mamy o automatyzacjach nocnych.
Znaczy
>> to jest tematikowy
już już to testowałem, aczkolwiek nie
wiem, nie wiem jak ty Krzyśku, ale ja
jestem zwolennikiem
jednak budowania swoich customowych
jakiś chron jobów. kontrolę na to.
>> Tak. A poza tym, poza tym to działa
tylko z poziomu cloud coda. A co jeśli
ja chcę na przykład, nie wiem, z poziomu
telefonu,
z jakiegoś innego narzędzia mieć też
możliwość dostępu do tego mojego
seconda,
który się wykonuje? No wtedy nie ma.
>> Jesteśmy uwięzieni wtedy, co nie?
Poza tym ja teraz budowanie takich
narzędzi z wykorzystaniem
clot codea to jest no relatywnie proste
na własne potrzeby i zbudowanie takich
rozwiązań, które się odpalają, nad
którymi mamy pełną kontrolę i jesteśmy w
stanie je integrować z czym chcemy i w
jaki sposób chcemy je dostosować jest
bajecznie proste.
>> Pełna zgoda. Pełna zgoda.
>> Kolejne pytanie. Jak praktycznie wygląda
wasza codzienna praca z second
oszczędzać czas? Czy można prosić o dwa
konkretne use casey od każdego z was? No
to co? Dawaj Krzychu jako pierwszy.
Jeśli chodzi o takie konkretne case na
pewno to, że jeśli pracuję nad praroma
projektami jednocześnie to dużo wiedzy
mi czy dużo, że tak powiem informacji
potrafi mi uciekać. Dużo rzeczy pojawia
się nowych. Dużo rzeczy też próbuję
gdzieś tam zapisać, zaplanować i też
potrafią mi uciekać. Yyy, co co to co ja
robię, nawet to co robiłem wcześniej w
ramach Notion, którego budowałem przez
trzy lata i teraz to co robię z
obsydianem, to to, że jeśli pojawia mi
się jakaś konkretna informacja, no
chociażby pomysł na jakiś nowy film, na
jakiś materiał, czy pojawia się jakiś
nowy feature, jakiś jakieś rozwiązanie,
które chciałbym się zapoznać, pierwsze
co robię, to mogę taką informację od
razu przerzucić sobie do takiego
seconda, do takiej bazy wiedzy. i
właśnie zrobić sobie z tego notatkę,
czyli już zostaje jakaś jakaś jakiś ślad
po tym, co zobaczyłem. Tak więc teraz
to, co służy, do czego służy ten
secondin, to on ma nam odciążyć trochę
tą naszą głowę. Bo jeśli my sobie
będziemy mówić, dobra zapamiętam to i
później do tego wrócę, to ja często mam
taką sytuację, że do tego nie wracam, bo
jest po prostu wylatuje to z głowy. Jest
za dużo tematów, jesteśmy nimi bardzo
przebodźcowani i właśnie budowanie
takiego second,
więc jesteśmy w stanie w tym secondinie
po prostu takie rzeczy sobie zrzucać,
syntetyzować, podsumowywać. No i to jest
taki pierwszy case. No drugi to jest na
pewno szybsze trawienie tych materiałów.
To żeby było jasne, nie chodzi też o to,
żeby delegować to myślenie do LLMów i
żeby one za nas trawiły tą wiedzę, a my
nic później z nią nie będziemy robić. No
trzeba oczywiście też czytać i
analizować w ogóle co się znajduje w tej
bazie wiedzy, no bo o to w tym chodzi.
Natomiast y dla mnie to jest też
uproszczenie, że mogę bardzo szybko
syntetyzować, podsumować sobie jakąś
wiedzę, zobaczyć pewne powiązania z tym,
co już wcześniej zgromadziłem. Może
jakieś tematy się łączą, różne koncepcje
mogą się na siebie najeżdżać. Może ta
jest słusżna, a może inna. Także to też
pozwala mi później to wszystko w ramach
takiego mojego, takiej mojej bazy wiedzy
sobie odbić i stwierdzić, czy to co na
przykład jakaś nowa informacja jest
słuszna, czy to jest coś nowego, czy to
może jest ten sam temat odgrzany kotlet,
ale troszeczkę w inny sposób. Więc to
też w ramach takiego secondweryfikować
pewne tematy i koncepcje. To to tak ode
mnie.
>> A to ja może uderzę w takim teraz
koncepcie biznesowym.
Oczywiście ja często biorę udział w
spotkaniach z klientami i jeśli klient
wyrazi zgodę, abym no mógł sobie nagrać
tą rozmowę, to ja właśnie nagrywam taką
rozmowę, która później trafia jako
transkrypcja do secondraina, na
podstawie której jest generowana notatka
z takim podsumowaniem, o czym
rozmawialiśmy, jakie są action itemy,
kolejne kroki i tak dalej do wykonania I
na podstawie yyy tej notatki jest yyy
pisany draft maila, który mogę sobie
wysłać do klienta. Więc to jest taki
jeden z casjów yyy w kontekście
biznesowym y m który używam. A druga
sprawa, jeśli chodzi o taki kontekst
biznesowy, to też często
właśnie mam tutaj taką całą bazę wiedzy
zebraną na temat
mnie, jakie realizuję projekty,
jaką mam grupę docelową, jak wygląda
mój, nie wiem, brand design i tym
podobne rzeczy. No i na plus jakieś
przykładowe pytania, odpowiedzi do
klientów. Yyy, tak samo na podstawie
tych transkrypcji można naprawdę mnóstwo
rzeczy z rozmów z klientami wyciągnąć.
No i teraz do tego wszystkiego ma dostęp
yyy mój model, na podstawie czego yyy ja
mogę odpowiadać też klientom na jakieś
pytania, które ich nurtują, tak w bardzo
szybki sposób yyy dostając się do moich
notatek. Więc to są takie dwa casy z m
życia biznesowego, tak? gdzie Krzysiek
pokazał bardziej na zasadzie yyy takiego
yyy content creatora, a ja bardziej
tutaj z perspektywy biznesowej.
>> M. Dobra, kolejne pytanie. Czego
używacie do odpalania y skedulowania na
przykład hooksów? Hooków. Ja używam tych
hooków, które są wbudowane w
w cloud code. Natomiast też pokazywałem,
że poza tymi hookami ja też mam jakieś
skrypty pythonowe czy skrypty
powershellowe, które pomagają mi choćby
śledzić jakiś katalog, bo przykładowo w
hookach code coda nie ma takiego, który
pozwalałby mi właśnie
ten cały czas monitorować ten katalog,
czy się pojawi w nim jakiś nowy plik.
Dlatego właśnie albo wykorzystujemy
skrypty powershellowe, albo pythonowe,
aby taką funkcjonalność sobie zapewnić.
>> Krzyśku, chciałbyś coś do dorzucić?
>> Ja może dodam, ja może dodam y to też,
co, co ja w jednym projekcie testuję. Ja
jestem w ekosystemie, pracuję Macowym,
Appleowym, więc i mam telefon z iOSem i
mam komputer z MacOSem. I teraz
korzystam również z chmury. I co ja
robię w ramach takiej chmury? To można
sobie wydzielić folder właśnie w ramach
waszego i
teraz ten folder może być równie dobrze
Voltem. Więc jeśli wprowadzacie jakieś
zmiany do tego Volta z poziomu iClouda,
czyli właśnie z poziomu telefonu, mogą
lądować jakieś notatki.
Możecie je edytować wtedy z różnych
miejsc, to on też później się
synchronizuje w ramach waszego
komputera. I to jest też mega fajne i
proste z tego powodu, że wtedy ten Volt
jest utrzymywany w tej konkretnej
chmurze. Oczywiście to jest kwestia
waszych preferencji, czy czy jesteście
za chmurą, czy nie. Natomiast to jest
też jedna z opcji jak można, że tak
powiem, synchronizować się na tych
różnych konkretnych narzędziach. I też
to co bardziej w tym temacie, co tutaj
podałeś o schedulowanie to właśnie to,
że jeśli mamy takie taki drive
przykładowo, to tutaj my nie dbamy o
samą, że tak powiem, nie musimy dbać
nawet o jakiś mechanizm synchronizacji.
No ale to się synchronizuje by default
po prostu przez, że tak powiem, różne
procesy, które się dzieją pod spodem,
tak, jeśli chodzi o synchronizację
takiej chmury. Także ja tutaj nie muszę,
że tak powiem, dokładać kolejnych
kroków, ale to się dzieje po prostu z
automatu. To jest jedna, że tak powiem z
koncepcji taka inna troszeczkę niż to co
ty pokazałeś, co nie? Tak tylko żeby dać
jakąś inną perspektywę.
>> Dobra, wygląda to mega prosperująco.
Tylko jak to zbudować? Mam nadzieję, że
w bonusie będzie pokazany krok po kroku.
Tak, w bonusie dostajecie takie prosty
>> prosty scenariusz, jak to zbudować krok
po kroku. Natomiast zapraszamy do
społeczności, gdzie tam pogłębimy ten
temat, pokażemy też pewnie jakieś rzeczy
z synchronizacją tych notatek między
telefonem a innymi urządzeniami. Można
wykorzystać. No i pewnie wiele wiele
innych rzeczy i też jeśli będzie takie
zapotrzebowanie od strony społeczności
to też pokażemy jak krok po kroku
dokładnie zbudować takie bardziej
zaawansowane rozwiązanie niż to co
dzisiaj pokazaliśmy.
W sumie tutaj widzę, że też się pojawiły
takie dyskusje, że tutaj jest to głównie
prezentacja,
że liczyli na część warsztatową. Tak,
była tutaj część warsztatowa. Aczkolwiek
w momencie, kiedy Klaudi już przez 17
dokładnie minut chyba jak dobrze
pamiętam robił syntezę, to było trzeba
jakoś tutaj ten czas zagospodarować i
wtedy to była idealna okazja, aby
wytłumaczyć jak ten cały koncept został
zbudowany. Podobnie tutaj u Krzyśka to
wyglądało.
>> Jasne, dokładnie, dokładnie. Więc pewne
rzeczy na live, że tak powiem, się
wydłużają, jeśli chodzi o to, no to
trzeba to wziąć pod uwagę.
>> Tak, ktoś tutaj w ogóle zauważył w
międzyczasie, że 50k tokenów poszło na
dwa źródła. No jak się przetwarza
właśnie takie dłuższe filmy na YouTubie
i tak dalej, to tam lubi to mieć sporo
tokenów. E, aczkolwiek jednak te
mechanizmy, które tam pokazałem, typu y,
te hooki, które tam się odpalały, m,
które robiły te transkrypcje,
i tak dalej, to one były, m,
realizowane na poziomie zero tokenów, bo
wykorzystywaliśmy albo napisy z
YouTubea, albo bibliotekę,
przepraszam, bibliotekę, lokalny model
Whispera, który robił transkrypcję.
Okej, przejdźmy tutaj dalej.
Tutaj od Wojtka pytanie: W jaki sposób
kontrolujesz cały proces Wiki
zadziałał i jakie daje wyniki, błędy,
halucynacje i tak dalej.
Ja rozumiem, że kontrolujesz właśnie
przez te reguły, zasady, które
zdefiniujesz w ramach po prostu tej
konstytucji tego twojego Volta. Tak?
Czyli to jest właśnie to, co
wypracowujesz w ramach skil, w ramach
twojego clod, czyli twojego głównego
mózgu projektu. Tam możesz wszystkie, że
tak powiem, zasady, reguły, jeśli chodzi
o inest, czyli przetrawienie, że tak
powiem, tych plików poprzez chociażby
wyłapywanie jakieś sytuacji, gdzie coś
jest właśnie niepoprawne albo czegoś nie
chcesz na przykład wrzucać do tego
Volta, poprzez query, czyli wyciąganie
tej informacji, lint czyli też
zarządzanie tą spójnością, możesz to
wszystko ustalić, że tak powiem, z
poziomu tych instrukcji. I co ważne, no
to ja też mam nawet takie rzeczy jak a
mam też nawet takie zasady, którymi też
się podzieliłem w ramach tego tego
bonusu. Mianowicie też takie coś jak
super session, czyli zastępowanie
wiedzy. Każda wiedza ma jakiś tam swój
life cycle, czyli jakiś tam okres
trwania, że tak powiem. nowe źródło może
zaprzeczyć po prostu staremu jakiemuś
założeniowi i wtedy nie kasujemy tej
wiedzy jawnie, ale po prostu ją
zastępujemy. Yyy, więc y też jesteśmy w
stanie zapisać po prostu w dwóch
miejscach, że po prostu taki nawet
callout w treści czytelny dla człowieka,
że słuchaj, ten materiał jest już
outdated, został zastąpiony nowym
materiałem, także też jesteś w stanie,
że tak powiem, aktualizować tą wiedzę i
nawet jeśli coś jest nieaktualne, to też
to zaznaczyć. y da się tym też śmiało.
To oczywiście jest dużo koncepcji. Ja
pokazuję też jedną ze swoich podejść. A
oczywiście można to robić w w inny
sposób, ale to też jest jakaś jedna
jedna opcja na to, jak można zarządzać
takimi y zadaniami. I to też to, co
powiedziałem wcześniej, czyli dla każdej
dla każdej Wiki to co ja robię to też
stosuję ten podział taki stopniowania
jeśli chodzi o confidence score, czyli
taki poziom pewności. Tak, im więcej mam
źródeł, które potwierdzają to samo
doniesienie, tym to jest dla mnie też
pewniejsze, że to wiki po prostu ma
wtedy ten confidence na wysokim poziomie
i to oznacza, że po prostu mogę temu
zaufać. Jak ma coś niski ten poziom, no
to znaczy, że nie ma na razie za dużo
dowodów albo coś jest niejasne i trzeba
by było to poddeprzeć jakimiś innymi
jeszcze materiałami. Także no to to są
różne koncepcje.
>> Dobra Krzychu, a ile czasu zajęło ci
zbudowanie tego braina?
Tak najwięcej w zbudowaniu w sensie
jeśli chodzi o sam notion, pobieranie
tych danych. Tutaj bardziej notion
traktuje jako sam już second brain w
sobie. Tutaj nie musiałem za dużo
edytować, no bo ja już jakąś strukturę
wypracowałem w ramach tego notion przez
te lata. Natomiast ten, no ten drugi
obsydian, który pokazywałem w ramach
tego researchu obsydianowego,
zajął mi tak naprawdę, szczerze mówiąc,
taki główny setup, najważniejsze rzeczy
jakoś około godzinki. Oczywiście to nie
było gdzieś tam pierwsze zderzenie. Już
z obsydianem sobie też pracowałem
wcześniej, natomiast takie najważniejsze
rzeczy byłem w stanie gdzieś tam do
godzinki sobie setapować już jakieś
pierwsze oczywiście źródła zaciągnąć,
przygotować, że tak powiem, instrukcje,
reguły, konkretne pluginy, z których
będę korzystał w ramach tego projektu i
też skille. Także to to myślę, że to
jest taka baza, fundament. No a później
to już jest tak naprawdę dalsza praca po
prostu z tym obsydianem. I jeśli chodzi
o o zbudowanie tego braina, no to ciężko
jest powiedzieć ile zajęło. No bo
pytanie czy pytasz o samą strukturę
wstępną, czy o całość. No bo wiadomo, że
ten mózg, ten ta nasza baza wiedzy
będzie ewoluować i on ewoluuje do
dzisiaj. Więc tak naprawdę,
>> ale powiedzmy ten silnik, powiedzmy ten
silnik,
który zbudowałeś, tak? Bo wiadomo, że
dodawanie źródeł to na bieżąco, ale sam
silnik.
>> Tak, tak, tak. No to myślę, że do
godzinki, żeby nawet gdzieś tam
wypracować jakąś koncepcję takie wiesz,
ja ja to co pokazałem w ramach tego
Obsidian Volta to jest bardzo prosta
struktura. Ja tutaj też nie mam jakiś,
że tak powiem, wodotrysków, jeśli chodzi
o jakieś dodatkowe integracje, tak jak
ty pokaz pokazałeś z różnymi
narzędziami. Mam integrację z websan
clipperem, mam oczywiście też chociażby
też synchronizację w innym projekcie z z
chmurą, no ale to zależy od konkretnego
projektu. A taki podstawowy projekt, no
to byłem w stanie dowieźć do godzinki.
Natomiast nie ukrywam, że teraz z
wypracowanymi instrukcjami tak naprawdę
tworzenie nowego Volta w innej tematyce
zajmuje mi o wiele szybciej. No bo biorę
gotowy template, nawet ten co pokazałem
w ramach y w ramach tych bonusów. No i
mogę już z nim sobie zacząć działać i
tam clot mnie prowadzi za rączkę i
wypytuje mnie konkretnie co chcę zrobić.
Także to idzie po prostu o wiele wiele
sprawniej. Yyy, oczywiście później
zbieranie tej wiedzy, no to żeby
zbudować taki konkretny second brain, no
to trzeba siedzieć i coś do niego, że
tak powiem, wrzucać, uzupełniać go,
jakieś informacje. Samo się to nie
zrobi. No może, że masz faktycznie
poautomatyzowane różne importy, to wtedy
może się
>> może się budować i sam. Pewnie
>> właśnie. Wiesz, ja po to stworzyłem
sobie RS feedy, które są zapięte na
tematy, które mnie interesują i one
zbierają informacje i po prostu raz
dziennie wrzucają materiały, które
przechodzą jeszcze przez filtr, o którym
wcześniej tam rozmawialiśmy, bo na
przykład, nie wiem, w tematach
finansowych mnie nie interesuje Forex,
tak więc po co mają mi tam lecieć i
przepalać też jakieś tokeny czy
cokolwiek
przy samej syntezie tych notatek.
Natomiast u mnie też to nie zajęło
długo. Ja tak naprawdę to co ja zrobiłem
to ja wziąłem Gista i Twita od
Karpatiego.
Wziąłem sobie Klaudiusza i powiedziałem:
"Dobra zaczynamy budować second code
plus Obsidian na podstawie koncepcji
właśnie Karpatieego. Tutaj masz te linki
i od razu, od razu mu po prostu
dorzuciłem, że hej stary, chciałbym po
prostu w tej koncepcji zautomatyzować
kilka rzeczy. daj mi kilka pomysłów. No
i dosłownie po 5, 10 minutach miałem już
rozpisane wstępnie
PRD, które przedstawia całą koncepcję
tego seconda wraz z kilkoma pomysłami na
automatyzację. Przedyskutowałem chwilkę
te
te automatyzacje. Stwierdziłem, dobra,
robimy jakieś OCR, robimy jakieś RS
feedy na automacie, robimy yyy dodatkowo
jakieś tam taski i tak dalej. No i w
zasadzie po jakieś 30, 40 minutach
miałem gotowe PRD, które następnie przez
kolejne 30 minut zostało
zaimplementowane przez Klaudiusza.
Oczywiście tam pojawiły się jakieś
drobne błędy, więc dwie, trzy iteracje i
po niespełnych dwóch godzinach miałem
gotowy silnik, który wam dzisiaj
pokazałem i następnie tylko
wygenerowałem jakieś fejkowe dane, aby
mieć na warsztat i
w sumie to szybko działać. do
realizacji.
>> Tak to jest nawet, bo czasami czasami mi
się wydaje, że za bardzo komplikujemy.
Często po prostu najprostsza metoda jest
dobra, żeby zacząć i to co
pokazywaliśmy, ja to też wrzuciłem. Ja
to już już mówię to któryś raz jak
mantrę wrzuciłem to w ramach materiałów
to, które macie na mailu. Tam jest
również link do Karpatiego, do tej
notatki, którą on wrzucił, która się
stała wiralem i ją też równie dobrze,
jeśli chcecie, możecie z nią zacząć, tak
jak powiedział Krzysiek, wrzucić po
prostu do cloda i zacząć z nim pracować.
albo skorzystać z tego templateu, który
ja już rozwinąłem gdzieś tam pod siebie,
albo zacząć od totalnego zera i
zobaczyć, czego wam tak naprawdę
brakuje. Także to jest piękne w tym
wszystkim, że każdy może sobie to
dostosować do swoich własnych potrzeb.
Nie ma jednej, że tak powiem,
sprawdzonej, idealnej, że tak powiem,
metody. Każdy musi sobie to dostosować
na swoje potrzeby.
>> Okej. Macie gdzieś udostępnione
narzędzia, które stosujecie swoich AI?
Akurat
jeśli
prawdopodobnie chodzi o projekty, w
których korzystamy i ja właśnie na
potrzeby społeczności buduję taki zbiór,
który na dniach wrzucę
rekomendowanych narzędzi przez nas oraz
alternatyw.
Więc w ramach społeczności pojawi się
taki bardzo rozbudowany zbiór
>> ja dużo buduję skillów i narzędzi takich
wokół tych moich projektów, z którymi
działam, które mogę reużywać, czyli nie
tworzę jednego, że tak powiem, jak robię
na przykład skillsy jakieś, to staram
się robić je tak, żeby móc je
wykorzystywać w wielu projektach
jednocześnie, czyli takie globalne, że
tak powiem, skille. To na przykład jest
też mega mega fajnym rozwiązaniem.
>> Ostatnie takie dwa pytania. Hmm, w sumie
na to już odpowiedzieliśmy wcześniej.
Czy można zainstalować Obsydiana w
chmurze i trzymać projekty w niej QR
Code?
>> O, popatrz, nawet nie czytałem tego,
przyznaję się.
>> I w zasadzie już yyy to wybrzmiało chyba
trzykrotnie.
>> Możesz sobie wę zainstalować na
iCloudzie też naze czy na VPSie, własnym
serwerze.
>> Tak. i macie dzięki temu yyy synka
między wszystkimi waszymi applowymi
urządzeniami.
A tu w ogóle pojawiło się pytanie: "Nie
lepiej właśnie używać Gemini?
Przynajmniej będzie mógł bez problemu
obejrzeć film z YouTube bez żadnych
dodatkowych narzędzi". E pytanie.
>> On też ma narzędzia pod spodem. To nie
jest tak, że to się dzieje magicznie. No
dalej ten model musi mieć jakieś
narzędzia.
>> Tak. pytanie, co realizujesz i pytanie,
czy jesteś aż tak bardzo bogaty, żeby
takie rozwiązanie sobie wprowadzić, bo
nie wiem, jeśli chcemy sobie stworzyć
transkrypcję, nawet używając Geminia
versus Geminiaa, aby obejrzał, zrozumiał
co się dzieje na filmie. A poza tym jest
pewien, ja sam się bawiłem, bo ja też
automatyzowałem choćby podcast, gdzie
wykrywałem emocje, inne rzeczy za pomocą
właśnie tego modelu geminajowego. No i
się pojawia pewien problem. Mniej więcej
przy około 30, 40 minutach zaczyna
halucynować. Co zrobisz, jeśli będziesz
miał dłuższy materiał? Druga sprawa,
przetworzenie takiego materiału
dwugodzinnego w przypadku podcastu
czasami potrafi już kosztować nawet
kilka dolarów po API.
No i pytanie, czy faktycznie chcesz
oglądać, rozumieć co się dzieje na
warstwie obrazów? Bo na warstwie obrazu
oczywiście możemy zobaczyć, że tam jest
czerwony samochód, jest jakaś ładna pani
i tak dalej, ale czy to jest potrzebne
tobie?
Ja już osobiście sam bym wolał zbudować
taki takie narzędzie. wziąć właśnie od
Googlea narzędzie, od Gemini yyy
multimodal embedding, gdzie sam bym
sobie przetworzył za pomocą lokalnych
modeli, bo można wykorzystać y lokalne
modele plus ten ich model embedingowy,
który jest właśnie dostępny jako open
source i w całości zrobić sobie darmowy
właśnie taki wektoryzację, dzięki czemu
też możemy rozmawiać i zrozumieć co się
dzieje na tym na tej warstwie. Więc ja
osobiście Geminia wolałbym nie używać,
bo już sam yyy używałem i przepaliłem
kilkanaście czy kilkadziesiąt dolarów
tylko na testy, a w zasadzie nic
konkretnego nie zostało zbudowane, a
problem za problemem się pojawiał
właśnie jak dłuższy materiał niż 30
minut, halucynacje i wiele innych
problemów, więc ja często jestem
zwolennikiem budowania nawet rozwiązań
oparte o lokalne narzędzia niż
m niż właśnie yy czasami korzystanie z
jakichś jakiś gotowców. Dobra, moi
drodzy, tutaj już tak przeglądając już
jakiś takich konkretnych pytań
nie widzę.
>> Oczywiście łapka w górę, jeśli
faktycznie jeszcze wytrwaliście z nami
tutaj i jesteście z nami już chyba dwie
godziny livea, tak? Nawet ponad. Także
>> fajnie tutaj dla wytrwałych. Jeszcze raz
dokładnie. Dziękujemy i polecamy się,
>> bo sporo, bo sporo pytań tutaj widzę
teraz, jak już do końca dyskusji jest
powtarzających się, czyli tematy, na
które już wcześniej odpowiedzieliśmy,
więc tutaj nie widzę już żadnych takich
pytań nowych,
więc no pozostaje nam się już tylko z
wami pożegnać, ale zanim to zrobimy, to
oczywiście
małe żebro lajkowanie,
czyli jeśli to co pokazaliśmy,
pokazaliśmy wam dzisiaj podoba się wam
to oczywiście
prośba o zostawienie po sobie śladu w
postaci subskrypcji, komentarza, lajka,
bo pozwala nam to
pozwala nam to
>> po prostu docierać do nowych osób, tak
samo
>> docierać do do nowych osób.
Także tutaj już
widzimy, że Marek
tutaj powiedział, że wykona akcję
lajkowania, więc tutaj dzięki Marku.
No i oczywiście dla wszystkich osób,
które dołączyły do nas, bo mamy kolejne,
że tak powiem, nowe osoby na pokładzie
AI Ninjas, także też za to dziękujemy.
I mam nadzieję, że po prostu ta
społeczność w ramach też te materiały,
które są w ramach społeczności wniosą
wam realną wiedzę i po prostu będziecie
mogli to wykorzystać w praktyce, w
swoich rozwiązaniach.
>> Ja tutaj jeszcze na czacie widziałem, że
w międzyczasie się pojawiło pytanie, czy
będzie kolejny live. Tak, będzie kolejny
kolejne spotkanie planujemy na maj.
Jeszcze
jeśli chodzi o jakieś konkrety, to
będziemy was informować na liście
mailowej. Dlatego też warto się zapisać
i być na bieżąco, bo na newsletterze też
dzielimy się ogromem wiedzy. No i
oczywiście zapraszamy was do dołączenia
do społeczności
i do jutra do 20 do 23:59 macie
możliwość dołączenia yyy w korzystnej
cenie obniżonej aż o 50 zł taniej, więc
yyy naprawdę to nie są duże pieniądze, a
w każdej chwili możecie zrezygnować.
Także macie 14 dni na wypróbowanie i
możecie do nas napisać bez podania
żadnej przyczyny, a my wam zwrócimy
pieniądze. Więc możecie sobie na
spokojnie przez dwa tygodnie
przetestować, czy społeczność A ninjas
jest dla was.
>> Chciałbyś też może dodam też
>> Ja tylko tak dodam na domknięcie. Nie
jesteśmy od wczoraj. Oczywiście ten na
na naszym kanale i też na na mailu
dostajecie też w tym pierwszym takim
powitalnym dostęp do poprzednich źródeł,
poprzednich materiałów. też w ramach
naszego kanału możecie prześledzić
poprzednie warsztaty. Także no to co
chcę też zaznaczyć, że nie jesteśmy od
wczoraj i też jutro nie znikamy, także
śmiało możecie też zapoznać się z
poprzednimi publikacjami. Tam też jest
dużo, dużo wiedzy do, że tak powiem,
skonsumowania odnośnie Cloda czy też
marketingu z AI, ale nawet i Open Clow,
który jest też dosyć świeżym tematem.
Yyy, nawet z tego co widzę to on tutaj
największym echem się odbił na naszym
kanale, także też do nich zapraszam. No
i widzimy się z niektórymi już w
społeczności. Także dzięki wielkie za
zaufanie.
jeszcze z innymi osobami pewnie za kilka
tygodni na kolejnym warsztacie i
oczywiście też zachęcamy do wypełniania
akient ankiet, bo oczywiście dzisiejszy
temat
został przez
>> przez społeczność, więc my staramy się
realizować materiały, które dla was są
potrzebne.
No dobra, to co, albo widzimy się z
częścią osób na społeczności, albo za
kilka tygodni na kolejnym otwartym
warsztacie.
Także wielkie dzięki za dzisiaj i do
usłyszenia. Hej,
>> dzięki wielkie. Cześć.