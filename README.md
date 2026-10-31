# Dealon: Sprint 1

Sprint 1 goal: a visitor can register, log in and log out, and search for a product to see
listings from several sources, loaded from the database through the four-layer structure.

## Run it (XAMPP, Windows)
1. Start **Apache** and **MySQL** in the XAMPP Control Panel.
2. Copy the `dealon` folder into `C:\xampp\htdocs\`.
3. Open http://localhost/phpmyadmin, click **Import**, choose `database/setup.sql`, click **Import**.
4. Open http://localhost/dealon/public/

## Run the tests
In a terminal inside the `dealon` folder:
    C:\xampp\php\php.exe tests\run.php --db

## Layers
- `app/Presentation`  controllers and views (HTML, forms, messages)
- `app/Business`      services and rules (all validation and decisions)
- `app/DataAccess`    repositories (the only place with SQL)
- MySQL               tables in `database/schema.sql`

Sample data only. Dealon does not sell products or process payments.
