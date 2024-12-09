# 📚 Systém správy knižnice pre STU

<img src="https://github.com/user-attachments/assets/261cea60-5a6c-463c-897b-d8ceb27cd499" width="60%" alt="Prehľad systému správy knižnice">

## 📑 Obsah
- [📖 Všeobecné Informácie](#📖-všeobecné-informácie)
- [✨ Funkcionality](#✨-funkcionality)
- [🛠️ Technológie](#🛠️-technológie)
- [📊 Model databázy](#📊-model-databázy)
- [🚀 Začiatok práce](#🚀-začiatok-práce)
  - [🔧 Požiadavky](#🔧-požiadavky)
  - [⚙️ Spustenie aplikácie](#⚙️-spustenie-aplikácie)
  - [📦 Kompilácia balíkov](#📦-kompilácia-balíkov)
  - [🗄️ Správa databázy](#🗄️-správa-databázy)
  - [✉️ Testovanie odosielania e-mailov](#✉️-testovanie-odosielania-e-mailov)
- [👥 Poďakovania](#👥-poďakovania)

## 📖 Všeobecné Informácie

Systém správy knižnice je webová aplikácia na správu knižnice. Umožňuje prehliadať katalóg knižnice a vykonávať operácie s knižničnými materiálmi a používateľmi. 📚👥

**Projekt vytvorený v rámci študijného seminára:**
- **Kurs:** IKT - Programovanie v Jave

## ✨ Funkcionality

### 👤 Správa používateľov
**Role (základ pre autorizáciu):**
- **Administrator**
- **Knižničár**
- **Čitateľ**

**Dostupné operácie:**
- 🆕 Vytvorenie používateľa (pridanie nového používateľa)
- ✏️ Úprava a aktualizácia údajov používateľa
- 🗑️ Odstránenie používateľa
- 🔐 Autentifikácia (prihlásenie/odhlásenie)
- 👀 Zobraziť všetkých používateľov (s vyhľadávaním, filtrovaním, triedením a stránkovaním)
- 📄 Zobraziť detaily používateľa pre konkrétneho používateľa
- 🧑‍💼 Zobraziť detaily aktuálneho používateľa (Moje údaje)

### 📚 Správa knižničných materiálov/zdrojov a katalógu

#### 🖋️ Autori
**Dostupné operácie:**

| Operácia                              | Obrázok                                                                                                  |
|---------------------------------------|----------------------------------------------------------------------------------------------------------|
| ➕ Pridať nového autora                | <img src="https://github.com/user-attachments/assets/08a97a4d-5300-40d2-9280-aeb256827765" width="50%" alt="Pridať autora"> |
| ✏️ Upraviť a aktualizovať autora       | <img src="https://github.com/user-attachments/assets/bfad4634-d17a-4fa9-a37d-c382e393a464" width="50%" alt="Upraviť autora"> |
| 🗑️ Odstrániť autora                   | <img src="https://github.com/user-attachments/assets/6d9a1fd4-c72d-45bb-bd67-c8ceee88a3ac" width="50%" alt="Odstrániť autora"> |
| 👀 Prezrieť všetkých autorov            | <img src="https://github.com/user-attachments/assets/c4f8dd5f-1592-4392-a6c9-523628dcf08c" width="50%" alt="Prezrieť autorov"> |

#### 🗂️ Kategórie
**Dostupné operácie:**

| Operácia                                 | Obrázok                                                                                                  |
|------------------------------------------|----------------------------------------------------------------------------------------------------------|
| ➕ Pridať novú kategóriu                   | <img src="https://github.com/user-attachments/assets/246accd2-1673-4287-9f16-e80530f5a025" width="50%" alt="Pridať kategóriu"> |
| ✏️ Upraviť a aktualizovať kategóriu      | <img src="https://github.com/user-attachments/assets/c19e047e-29ac-4fd7-b474-ab6421277034" width="50%" alt="Upraviť kategóriu"> |
| 🗑️ Odstrániť kategóriu                    | <img src="https://github.com/user-attachments/assets/d241ba90-394b-4713-81d7-648d72547f4c" width="50%" alt="Odstrániť kategóriu"> |
| 👀 Prezrieť všetky kategórie              | <img src="https://github.com/user-attachments/assets/0c7a694c-b0f7-469f-b9ee-7fadc1bf1f7f" width="50%" alt="Prezrieť kategórie"> |

#### 📖 Diela
**Dostupné operácie:**

| Operácia                              | Obrázok                                                                                                  |
|---------------------------------------|----------------------------------------------------------------------------------------------------------|
| ➕ Pridať nové dielo                   | <img src="https://github.com/user-attachments/assets/a059b3e2-ab33-477c-8ed3-0a80eb4ace5c" width="50%" alt="Pridať dielo"> |
| ✏️ Upraviť a aktualizovať dielo       | <img src="https://github.com/user-attachments/assets/f69d3439-13fe-472c-8d29-d0747d149c5d" width="50%" alt="Upraviť dielo"> |
| 🗑️ Odstrániť dielo                    | <img src="https://github.com/user-attachments/assets/c0d99208-365c-400f-8a48-6a5810f6c3cb" width="50%" alt="Odstrániť dielo"> |
| 👀 Prezrieť všetky diela               | <img src="https://github.com/user-attachments/assets/c6efb7a2-2cc3-4b9e-b267-246b637e0c8d" width="50%" alt="Prezrieť diela"> |
| 📦 Prezrieť všetky kópie kníh konkrétneho diela | <img src="https://github.com/user-attachments/assets/bbeb797f-e026-4d05-9b57-3e70fd2757c7" width="50%" alt="Prezrieť kópie kníh"> |

#### 📕 Knihy
**Dostupné operácie:**

| Operácia                                | Obrázok                                                                                                  |
|-----------------------------------------|----------------------------------------------------------------------------------------------------------|
| ➕ Pridať novú knihu                     | <img src="https://github.com/user-attachments/assets/17322869-09a7-41d0-a258-6fdf34b7403d" width="30%" alt="Pridať knihu"> |
| ✏️ Upraviť a aktualizovať knihu         | <img src="https://github.com/user-attachments/assets/af9adfe8-cc7a-4258-9133-9554bb52902c" width="30%" alt="Upraviť knihu"> |
| 🗑️ Odstrániť knihu                      | <img src="https://github.com/user-attachments/assets/b7374475-4a5a-4a68-949a-c071334d5706" width="30%" alt="Odstrániť knihu"> |
| 👀 Prezrieť všetky knihy                | <img src="https://github.com/user-attachments/assets/9b939fe6-fa45-40cd-9d65-ef26fdac0686" width="30%" alt="Prezrieť knihy"> |

### 🔄 Výpožičky zdrojov - Pôžičky

| Operácia                                  | Obrázok                                                                                                  |
|-------------------------------------------|----------------------------------------------------------------------------------------------------------|
| 🆙 Začať pôžičku                           | <img src="https://github.com/user-attachments/assets/7dcf260e-c53b-441f-958b-8485e316d49b" width="50%" alt="Začať pôžičku"> |
| 🏁 Dokončiť pôžičku                        | <img src="https://github.com/user-attachments/assets/002f69e4-ced9-46d8-ba1a-16a87a1ab270" width="50%" alt="Dokončiť pôžičku"> |
| 📚 Prezrieť všetky pôžičky konkrétnej knihy | <img src="https://github.com/user-attachments/assets/e86e8e6c-74e5-4807-ac9e-564cc8fa4ea2" width="50%" alt="Prezrieť pôžičky konkrétnej knihy"> |
| 👥 Prezrieť pôžičky podľa čitateľa        | <img src="https://github.com/user-attachments/assets/8af57a67-3454-4e5b-94b3-94381af66e28" width="50%" alt="Prezrieť pôžičky podľa čitateľa"> |

### 📧 Odosielanie e-mailových oznámení
- 📩 Odoslať e-mail "Vitajte" používateľovi pri vytvorení jeho účtu
- 📬 Odoslať e-mail "Pôžička začatá" čitateľovi pri výpožičke knihy
- 📥 Odoslať e-mail "Pôžička dokončená" čitateľovi pri vrátení knihy

## 🛠️ Technológie

- **Backend:** Java, Spring Boot, Spring Security
- **Frontend:** Thymeleaf, Bootstrap, HTML5, CSS3, JavaScript, jQuery
- **Databáza:** Flyway, PostgreSQL
- **Kontajnerizácia:** Docker
- **IDE:** IntelliJ IDEA

## 📊 Model databázy

![Model databázy](https://github.com/user-attachments/assets/9ed7b02b-569b-4765-95c3-d8f83b00bfbe)

Databáza pre Systém správy knižnice sa skladá z nasledujúcich tabuliek a ich vzťahov:

### **Tabuľky a ich polia**

1. ### 🗂️ **category**
   | Pole       | Typ           | Popis                                 |
   |------------|---------------|---------------------------------------|
   | `id`       | integer (PK)  | Jedinečný identifikátor kategórie      |
   | `name`     | varchar       | Názov kategórie                        |

2. ### 🖋️ **work**
   | Pole           | Typ           | Popis                                 |
   |----------------|---------------|---------------------------------------|
   | `id`           | integer (PK)  | Jedinečný identifikátor diela          |
   | `title`        | varchar       | Názov diela                           |
   | `description`  | varchar       | Popis diela                           |

3. ### 👤 **author**
   | Pole         | Typ           | Popis                                 |
   |--------------|---------------|---------------------------------------|
   | `id`         | integer (PK)  | Jedinečný identifikátor autora         |
   | `first_name` | varchar       | Meno autora                            |
   | `last_name`  | varchar       | Priezvisko autora                      |

4. ### 📚 **book**
   | Pole                 | Typ           | Popis                                  |
   |----------------------|---------------|----------------------------------------|
   | `id`                 | integer (PK)  | Jedinečný identifikátor knihy           |
   | `work_id`            | integer (FK)  | Odkaz na dielo                          |
   | `publisher_name`     | varchar       | Názov vydavateľa                        |
   | `year_of_publishing` | timestamp     | Rok vydania                             |
   | `isbn`               | varchar       | ISBN knihy                              |
   | `book_status`        | status        | Stav knihy                              |
   | `available`          | boolean       | Dostupnosť knihy                        |

5. ### 👥 **user**
   | Pole             | Typ           | Popis                                   |
   |------------------|---------------|-----------------------------------------|
   | `id`             | integer (PK)  | Jedinečný identifikátor používateľa      |
   | `first_name`     | varchar       | Meno používateľa                         |
   | `last_name`      | varchar       | Priezvisko používateľa                   |
   | `password`       | varchar       | Heslo používateľa                        |
   | `email`          | varchar       | Email používateľa                         |
   | `date_of_birth`  | timestamp     | Dátum narodenia                           |
   | `contact_number` | varchar       | Kontaktné číslo                           |
   | `enabled`        | boolean       | Stav aktivácie                            |

6. ### 📝 **loan**
   | Pole             | Typ           | Popis                                   |
   |------------------|---------------|-----------------------------------------|
   | `id`             | integer (PK)  | Jedinečný identifikátor pôžičky          |
   | `member_id`      | integer (FK)  | Odkaz na čitateľa                         |
   | `librarian_id`   | integer (FK)  | Odkaz na knižničára                      |
   | `book_id`        | integer (FK)  | Odkaz na knihu                            |
   | `date_issued`    | timestamp     | Dátum vydania                             |
   | `date_returned`  | timestamp     | Dátum vrátenia                            |

7. ### 🔐 **role**
   | Pole    | Typ           | Popis                                    |
   |---------|---------------|------------------------------------------|
   | `id`    | integer (PK)  | Jedinečný identifikátor role             |
   | `name`  | varchar       | Názov role (Admin, Librarian, Member)    |

8. ### 🔗 **user_role**
   | Pole      | Typ           | Popis                                   |
   |-----------|---------------|-----------------------------------------|
   | `user_id` | integer (FK)  | Odkaz na používateľa                     |
   | `role_id` | integer (FK)  | Odkaz na rolu                             |

9. ### 🔗 **work_author**
   | Pole        | Typ           | Popis                                 |
   |-------------|---------------|---------------------------------------|
   | `work_id`   | integer (FK)  | Odkaz na dielo                          |
   | `author_id` | integer (FK)  | Odkaz na autora                          |

10. ### 🔗 **work_category**
    | Pole          | Typ           | Popis                                 |
    |---------------|---------------|---------------------------------------|
    | `work_id`     | integer (FK)  | Odkaz na dielo                          |
    | `category_id` | integer (FK)  | Odkaz na kategóriu                       |

---

### 🔗 **Vzťahy medzi tabuľkami**

1. **work_author**:  
   - `work_id` ↔️ `work.id`  
   - `author_id` ↔️ `author.id`  

2. **work_category**:  
   - `work_id` ↔️ `work.id`  
   - `category_id` ↔️ `category.id`  

3. **book**:  
   - `work_id` ↔️ `work.id`  

4. **loan**:  
   - `member_id` ↔️ `user.id` (čitateľ)  
   - `librarian_id` ↔️ `user.id` (knižničár)  
   - `book_id` ↔️ `book.id`  

5. **user_role**:  
   - `user_id` ↔️ `user.id`  
   - `role_id` ↔️ `role.id`  

---

### 📝 **Kľúčové momenty**

- **Primárne kľúče (PK)** zaručujú jedinečnosť záznamov v každej tabuľke.
- **Cudzí kľúče (FK)** zabezpečujú vzťahy medzi tabuľkami a udržiavajú integritu údajov.
- **Role a používatelia** sú prepojení cez medzistátnu tabuľku `user_role` pre implementáciu autorizácie.
- **Pôžičky (loan)** prepojujú knihy, čitateľov a knižničárov, sledovaním výpožičiek a vrátení kníh.
- **Knihy (book)** sú prepojené s dielami (work) a môžu mať viacero kategórií a autorov cez tabuľky `work_category` a `work_author`.

## 🚀 Začiatok práce

### 🔧 Požiadavky
Je potrebné nainštalovať nasledujúce:
- **Docker** spolu s **docker-compose**
- **Java Development Kit (JDK)**
- **Maven** (ak sa nepoužíva poskytovaný Maven Wrapper)

### ⚙️ Spustenie aplikácie
Vykonajte nasledujúce príkazy v termináli:

1. **Prejdite do zložky projektu (vykonáva sa z koreňového adresára repozitára):**
    ```bash
    cd library-management-system/
    ```
    ![Prejsť do zložky projektu](https://github.com/user-attachments/assets/37016f78-70c8-47ed-8381-e0ee26ef1ff2)
  
2. **Zostavte `.jar` súbor projektu v priečinku `target`:**
    ```bash
    ./mvnw clean package -DskipTests
    ```
    ![Zostavenie projektu Maven](https://github.com/user-attachments/assets/f3351b46-dfec-4263-b456-2753d52c0cda)
  
3. **Zostavte a spustite Docker prostredie a lokálny webový server:**
    ```bash
    docker-compose up
    ```
    *(Zastaviť môžete pomocou `Ctrl+C`)*
    ![Spustenie Docker Compose](https://github.com/user-attachments/assets/76c166a1-167c-4154-bb0d-7f50920e655f)
  
4. **Otvorte aplikáciu v prehliadači:**
    [http://localhost:8080/](http://localhost:8080/)
  
**Ak potrebujete zmeniť kód a aplikovať zmeny:**

1. **Zastavte a odstráňte Docker kontajnery a ich objemy:**
    ```bash
    docker-compose down
    ```
    ![Zastavenie Docker Compose](https://github.com/user-attachments/assets/c6d0bdb3-7051-409a-8b25-0168b09858e3)
  
2. **Odstráňte Docker obraz `library-management-system.jar`:**
    ```bash
    docker rmi library-management-system.jar
    ```
    ![Odstránenie Docker obrazu](https://github.com/user-attachments/assets/75961e05-d158-4a25-9c96-d4726f2b0f9c)
  
3. **Opakujte kroky 2-4.**

### 📦 Kompilácia balíkov

Môžete vytvoriť inštalačné balíky `.deb` a `.rpm` pomocou `jpackage`. Pre tento účel vykonajte nasledujúce kroky:

#### 📥 Predbežné požiadavky

- **Pre kompiláciu `.deb` balíka:**
  - Nainštalujte `fakeroot`:
    ```bash
    sudo apt-get update
    sudo apt-get install fakeroot
    ```
  
- **Pre kompiláciu `.rpm` balíka:**
  - Nainštalujte `rpm-build`:
    ```bash
    sudo apt-get update
    sudo apt-get install rpm
    ```

#### 🏗️ Kompilácia `.deb` balíka
Vykonajte nasledujúci príkaz z koreňového adresára projektu:
```bash
jpackage --input target \
    --name LibraryManagementSystem \
    --main-jar library-management-system.jar \
    --type deb \
    --icon assets/images/icon.png \
    --dest out_dir
```
![Kompilácia .deb balíka](https://github.com/user-attachments/assets/f2bd103d-8791-4944-b36f-b85de15f9903)

#### 🏗️ Kompilácia `.rpm` balíka
Vykonajte nasledujúci príkaz z koreňového adresára projektu:
```bash
jpackage --input target \
    --name LibraryManagementSystem \
    --main-jar library-management-system.jar \
    --type rpm \
    --icon assets/images/icon.png \
    --dest out_dir
```
![Kompilácia .rpm balíka](https://github.com/user-attachments/assets/fc2f13eb-507d-43f8-8652-43214d64e8da)

#### 🛠️ Dodatočné možnosti
- `--app-version`: Určte verziu aplikácie.
- `--icon`: Pridajte ikonu aplikácie (napr. `icon.png`).
- `--dest`: Určte adresár pre uloženie vytvoreného balíka.

**Príklad s ikonou:**
```bash
jpackage --input target \
    --name LibraryManagementSystem \
    --main-jar library-management-system.jar \
    --type deb \
    --icon assets/images/icon.png \
    --dest out_dir
```

**Poznámky:**
- Uistite sa, že máte nainštalovaný JDK verzie 14 alebo vyššej, ktorý obsahuje `jpackage`.
- `jpackage` vytvára inštalačné balíky pre platformu, na ktorej je spustený. Pre vytvorenie `.rpm` balíka sa odporúča používať systémy založené na RPM (napr. Fedora alebo CentOS).

### 🗄️ Správa databázy
Databázu PostgreSQL môžete prezerať v okne databázy IntelliJ IDEA nasledovne:

1. **Prejdite do:** `View -> Tool Windows -> Database`
2. **Pridajte nový zdroj údajov:**
    - Kliknite na tlačidlo `+`
    - Vyberte `Data Source from URL` a zadajte nasledujúce údaje:

    **URL:** `jdbc:postgresql:///postgres`  
    **Driver:** `PostgreSQL`

3. **Nastavte vlastnosti pripojenia:**
    - **Username:** `postgres`
    - **Password:** `postgres`
    - **Database:** `postgres`
    - **Host:** `localhost`
    - **Port:** `5432`

### ✉️ Testovanie odosielania e-mailov
**MailHog Web UI**, nástroj na testovanie odosielania e-mailov vývojármi, je dostupný na adrese: [http://localhost:8025/](http://localhost:8025/)
![MailHog Web UI](https://github.com/user-attachments/assets/5438a75d-b280-4aac-94cb-839e52d39aed)

## 👥 Poďakovania

**Vedúci projektu, Senior Developer, Hlavný Architekt, Technický Riadiaci, Manažér pre kávu, Guru databázy, Testovací Inžinier, Deployment Špecialista, Dizajnér rozhraní, Server Administrator, Hlavný motivátor, Zodpovedný za meme, Oracle systému, Vládca bugov, Kódovacia legenda, Tanečný Výkon, Čarodej commitov, Safe-provider produkcie, Kráľ konzoly, Najvyšší vládca logov, Lokátor stratených bodkočiark, Master mergeov, Dokumentátor chaosu, Lomenač produkcie (v piatok), Špecialista na "funguje na mojom počítači", Vládca vetiev, Strážca deployment kľúčov, Zbierateľ stack traceov:**
- **Aleksandr Murzin** 😘

---

**Programovanie v Jave**  
**Fakulta elektrotechniky a informačných technológií STU v Bratislave**

---
