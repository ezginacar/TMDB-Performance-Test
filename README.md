# TMDB Performance Test Plan
This repo contains a simple performance testing template of TMDB (The Movie Database) for most visited pages

### **Public Endpoints**
- **GET `/movie/popular`** : Fetches a list of the most popular items.
- **GET `/tv/popular`** : Fetches a list of the most popular items.
- **GET `/trending/all`** : Fetches a list of the most popular movies,tvs,persons
- **GET `/movie/movie_id`** : Fetches a single movie

## Prerequisites

- **Apache JMeter**: Download and install from [JMeter's official website](https://jmeter.apache.org/).
- **Java**: Ensure Java 8 or higher is installed and configured.
- **Clone this repo**:
   ```bash
   git clone https://github.com/ezginacar/TMDB-Performance-Test

## Running The Test Plan

**Using JMeter GUI**
- Open Apache JMeter.
- Load the test plan file (TMDB_Performance_Test.jmx) via File > Open.
- Configure the required parameters, such as the number of threads (users) and ramp-up period, in the Thread Group section.
- Run the test by clicking the green Start button.

** Using JMeter CLI (Non-GUI Mode) **
- Open a terminal or command prompt.
- Navigate to the JMeter bin directory.
   ```bash
   jmeter -n -t TMDB_Performance_Test.jmx -l results.jtl
  
**Analyzing Reports**
- The test plan and related resources can also be accessed via Google Drive:
https://drive.google.com/drive/folders/1Eo2QtHKDpa-O62ChranLnqE7YApRb6R-

   ```bash
   jmeter -g /your/desired/path/results.jtl -o /your/desired/path/html_reports/



