# moers-hackday

All you need to know to use Diffix anonymization for the Moers Hackday

## Data set

The data set for the Moers Hackday consists of several years of traffic violations, both moving and stationary. The basic information for the data set is taken from [Moers Open Data](https://www.offenesdatenportal.de/organization/moers) (see [this page](https://www.offenesdatenportal.de/organization/20a7743d-057b-4e0e-a341-cf0adaf1502a?groups=transport-verkehr&tags=Bu%C3%9Fgelder)).

Moers removed all personal information from the data set. This makes the dataset private, but results in the loss of some potentially information about the data: How many different people have been fined? How many fines do different people have? Where do the people come from? What are their demographics?

Diffix allows us to learn this kind of information while still protecting privacy. Do demonstrate this, we have *added* synthetic data about persons to the Moers data: age, gender, and license-plate number. Diffix generates statistical information about the data set (including the people) without revealing individual information about the people.

## Tools

The [Open Diffix](https://open-diffix.org) project offers two tools for analyzing data anonymized by Diffix. **Diffix for Desktop** is a simple GUI-based desktop tool that runs on Windows, Mac, or Linux. **Diffix for PostgreSQL** is a PostgreSQL extension `pg_diffix` that anonymizes SQL queries. Diffix for PostgreSQL has more query features than Diffix for Desktop.

Diffix for Desktop is designed to be used by a *trusted* analyst. All of the personal information in the data set is visible to the analyst when using the tool.

Diffix for PostgreSQL can be used by anyone, including the public. It hides personal information.

## Diffix for Desktop

To analyze the data using Diffix for Desktop, do the following:

1. Download [Diffix for Desktop](https://www.open-diffix.org/download).
2. Download `moers.csv.zip` from this GitHub repo.
3. Unzip `moers.csv.zip` to make `moers.csv`.
4. After starting Diffix for Desktop, load `moers.csv` into the application.
5. Configure the **AID** to be the column `PID`

Now you are ready to analyze the data set.
