# Blogovací Web

## Popis projektu

Tento projekt je blogovací web vytvořený pomocí C# a .NET 8.0, s využitím databáze Microsoft SQL Server (MSSQL) na místním hostiteli. Webová aplikace umožňuje uživatelům procházet blogy, vytvářet nové příspěvky, editovat je a mazat.

## Funkcionality

- **Procházení blogů**: Uživatelé mohou prohlížet seznam blogů bez nutnosti přihlášení.
- **Vytváření příspěvků**: Pro vytvoření nového blogového příspěvku je vyžadováno přihlášení.
- **Editace příspěvků**: Přihlášení uživatelé mohou upravovat své vlastní blogové příspěvky.
- **Mazání příspěvků**: Přihlášení uživatelé mohou mazat své blogové příspěvky.
- **Zobrazení detailů příspěvku**: Každý blog obsahuje nadpis, datum publikace, označení zda je příspěvek připnutý, perex a text příspěvku.

## Technologie

- **Backend**: C# a .NET 8.0
- **Frontend**: HTML, CSS, JavaScript (vyžaduje vhodnou integraci pro správné zobrazení a interakci)
- **Databáze**: Microsoft SQL Server (MSSQL)
- **Autentizace**: Implementováno pomocí ASP.NET Identity pro správu uživatelů a jejich přihlášení

## Instalace a Spuštění

1. **Klonujte repozitář**:
    ```bash
    git clone https://github.com/uživatel/vaš-repozitář.git
    ```

2. **Nainstalujte závislosti**:
    Ujistěte se, že máte nainstalovaný .NET 8.0 SDK. V kořenovém adresáři projektu spusťte:
    ```bash
    dotnet restore
    ```

3. **Nastavte databázové připojení**:
    Upravte konfigurační soubor `appsettings.json` a nastavte připojení k vaší MSSQL databázi.

4. **Migrace databáze**:
    Spusťte migrace databáze, aby se vytvořily potřebné tabulky:
    ```bash
    dotnet ef database update
    ```

5. **Spusťte aplikaci**:
    ```bash
    dotnet run
    ```

    Webová aplikace bude dostupná na [http://localhost:5000](http://localhost:5000) nebo portu, který jste nakonfigurovali.

## Použití

- **Registrace a Přihlášení**: Uživatelé se mohou registrovat a přihlašovat prostřednictvím standardního registračního a přihlašovacího formuláře.
- **Správa příspěvků**: Po přihlášení mohou uživatelé přidávat nové příspěvky, upravovat existující a mazat je.

## Přispění

Pokud chcete přispět k tomuto projektu, můžete:

1. **Forknout repozitář**
2. **Vytvořit novou větev** (`git checkout -b vylepseni`)
3. **Provést změny a commitnout je** (`git commit -am 'Přidáno nové vylepšení'`)
4. **Pushnout změny do svého forku** (`git push origin vylepseni`)
5. **Odeslat Pull Request** do hlavního repozitáře

## License

Tento projekt je licencován pod [MIT License](LICENSE).

## Kontakt

Pro další informace nebo otázky mě můžete kontaktovat na [email@example.com](mailto:email@example.com).