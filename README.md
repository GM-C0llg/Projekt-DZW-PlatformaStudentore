# Udhëzues për Përdorimin e GitHub Desktop

## 1. Qëllimi

Ky dokument përmban udhëzimet për përdorimin e GitHub Desktop gjatë zhvillimit të projektit në lëndën **Dizajni dhe Zhvillimi i Uebit**.

Të gjithë anëtarët e grupit duhet t'i ndjekin këta hapa për të siguruar që ndryshimet në projekt ruhen dhe sinkronizohen saktë.

## 2. Shkarkimi i projektit (Clone)

Ky proces kryhet vetëm një herë, kur projekti shkarkohet për herë të parë në kompjuter.

1. Hapni **GitHub Desktop**.
2. Zgjidhni **File → Clone Repository**.
3. Në seksionin **GitHub.com**, gjeni repository-n e projektit.
4. Te **Local Path**, zgjidhni vendndodhjen ku dëshironi ta ruani projektin.
5. Klikoni **Clone**.

Tani projekti gjendet në kompjuterin tuaj dhe mund të filloni punën.

**Kujdes:** Nuk është e nevojshme të krijoni repository të ri. Të gjithë anëtarët punojnë me të njëjtin repository në GitHub, por secili ka kopjen e vet lokale.

## 3. Kontrollimi i ndryshimeve (Fetch Origin)

**Fetch Origin** kontrollon nëse ekzistojnë ndryshime të reja në GitHub.

Hapat:

1. Hapni GitHub Desktop.
2. Zgjidhni repository-n e projektit.
3. Klikoni **Fetch Origin** në pjesën e sipërme.
4. Prisni derisa të përfundojë kontrollimi.

Fetch nuk i bashkon automatikisht ndryshimet e reja me skedarët tuaj lokalë.

## 4. Marrja e ndryshimeve (Pull Origin)

**Pull Origin** i merr ndryshimet e reja nga GitHub dhe i integron në projektin tuaj lokal.

Hapat:

1. Klikoni **Fetch Origin**.
2. Nëse ka ndryshime të reja, GitHub Desktop do të shfaqë **Pull Origin**.
3. Klikoni **Pull Origin**.
4. Ndryshimet do të integrohen në projektin tuaj.

**Rregull i rëndësishëm:** Para se të filloni punën, gjithmonë kontrolloni nëse ka ndryshime të reja dhe bëni Pull kur është e nevojshme.

## 5. Ruajtja e ndryshimeve (Commit)

**Commit** përdoret për të regjistruar ndryshimet në historikun lokal të projektit.

Hapat:

1. Hapni projektin në editorin tuaj (p.sh. VS Code).
2. Bëni ndryshimet e nevojshme në kod.
3. Ruani skedarët (Ctrl + S).
4. Hapni GitHub Desktop.
5. Në seksionin **Changes**, shikoni skedarët që janë ndryshuar.
6. Sigurohuni që janë përzgjedhur skedarët që dëshironi t'i përfshini në Commit.
7. Te fusha **Summary**, shkruani një përshkrim të shkurtër të ndryshimeve.
8. Klikoni **Commit to main** (ose emrin e degës ku po punoni).

Shembuj të mesazheve:

- `Shtimi i faqes kryesore`
- `Krijimi i stilizimit CSS`
- `Rregullimi i navigimit`
- `Shtimi i funksionalitetit JavaScript`

**Kujdes:** Commit i ruan ndryshimet vetëm në repository-n lokal. Ato nuk janë ngarkuar ende në GitHub.

## 6. Ngarkimi i ndryshimeve (Push Origin)

**Push Origin** i ngarkon commit-et lokale në repository-n online në GitHub.

Hapat:

1. Pasi të keni përfunduar Commit, klikoni **Push Origin**.
2. Prisni derisa të përfundojë ngarkimi.
3. Hapni repository-n në faqen e GitHub për të verifikuar ndryshimet.

Pas këtij veprimi, anëtarët e tjerë mund t'i marrin ndryshimet tuaja përmes Pull.

**Kujdes:** Gjithmonë bëni Push pas Commit kur dëshironi që puna juaj të jetë e disponueshme për grupin.

## 7. Rrjedha e zakonshme e punës

Çdo anëtar duhet ta ndjekë këtë rend gjatë punës në projekt:

| Hapi | Veprimi      | Qëllimi                           |
| ---- | ------------ | --------------------------------- |
| 1    | Fetch Origin | Kontrolloni ndryshimet e reja     |
| 2    | Pull Origin  | Merrni ndryshimet nëse ekzistojnë |
| 3    | Edit         | Punoni në skedarët e projektit    |
| 4    | Save         | Ruani skedarët në editor          |
| 5    | Commit       | Regjistroni ndryshimet lokale     |
| 6    | Push Origin  | Ngarkoni ndryshimet në GitHub     |

**Mbani mend:**

Fetch → Pull → Edit → Save → Commit → Push

Nëse nuk ka ndryshime të reja, Pull nuk është i nevojshëm.

## 8. Si të shikoni historikun e ndryshimeve (History)

GitHub Desktop ruan historikun e commit-eve.

Për ta kontrolluar:

1. Hapni GitHub Desktop.
2. Zgjidhni repository-n.
3. Klikoni në seksionin **History**.
4. Shikoni commit-et dhe skedarët që janë ndryshuar.

Kjo ju ndihmon të identifikoni ndryshimet e bëra gjatë zhvillimit të projektit.

## 9. Konfliktet gjatë bashkëpunimit (Merge Conflicts)

Konfliktet mund të ndodhin kur dy anëtarë modifikojnë të njëjtën pjesë të një skedari.

Për t'i shmangur:

- Bëni Fetch dhe Pull para fillimit të punës.
- Mos modifikoni të njëjtën pjesë të kodit njëkohësisht pa koordinim.
- Bëni Commit dhe Push rregullisht.
- Informoni anëtarin tjetër kur ndryshoni skedarë të përbashkët.

Nëse ndodh një konflikt:

1. Lexoni mesazhin që shfaq GitHub Desktop.
2. Hapni skedarin që ka konflikt në editor.
3. Kontrolloni ndryshimet e të dy anëtarëve.
4. Vendosni cilat ndryshime duhet të ruhen.
5. Ruani skedarin e korrigjuar.
6. Shënoni konfliktin si të zgjidhur dhe përfundoni bashkimin sipas udhëzimeve të GitHub Desktop.

**Mos i fshini ndryshimet e anëtarit tjetër pa marrëveshje.**

## 10. Rregullat e bashkëpunimit

1. Çdo anëtar duhet të punojë në kopjen e vet lokale të repository-t.
2. Çdo anëtar duhet të respektojë strukturën e dosjeve të projektit.
3. Para fillimit të punës duhet të kontrollohen ndryshimet e reja.
4. Çdo Commit duhet të ketë një përshkrim të qartë.
5. Pas përfundimit të detyrës duhet të bëhet Push.
6. Ndryshimet në skedarët e përbashkët duhet të koordinohen.
7. Nuk duhet të fshihen ose të riemërtohen skedarët e anëtarëve të tjerë pa marrëveshje.
8. Nuk duhet të përdoret Force Push pa koordinim.
9. Para ngarkimit, kodi duhet të testohet.
10. Problemet teknike duhet t'u komunikohen anëtarëve të grupit.

---

## 11. Dallimet ndërmjet komandave

| Komanda | Funksioni                                               |
| ------- | ------------------------------------------------------- |
| Clone   | Shkarkon repository-n për herë të parë                  |
| Fetch   | Kontrollon dhe merr informacionin për ndryshimet e reja |
| Pull    | Merr dhe integron ndryshimet nga GitHub                 |
| Commit  | Regjistron ndryshimet në repository-n lokal             |
| Push    | Ngarkon commit-et lokale në GitHub                      |
| History | Shfaq historikun e commit-eve                           |

**Shënim përfundimtar:** GitHub Desktop mundëson përdorimin e këtyre funksioneve përmes ndërfaqes grafike, pa pasur nevojë të shkruhen komanda në terminal.
