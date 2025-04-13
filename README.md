### Repository Overview

The `PharmaTariffStrategyDashboard` is an R Shiny app analyzing pharmaceutical manufacturing strategies to minimize EU tariff exposure, with interactive visuals for global operations, tariff scenarios, and phased rollouts. Built for supply chain and sales professionals, it demonstrates Qore.AI’s potential to deliver data-driven clarity—akin to tackling automotive D&H cost surges (e.g., Suburban’s $995 to $2,195). The repo includes modular code, three branded logos, and a polished UI, making it a compelling case for analytics that “sell” outcomes.

### Repository Structure

```
PharmaTariffStrategyDashboard/
├── app.R                    # Main Shiny app
├── data/                    # CSV datasets
│   ├── locations.csv        # Global pharma locations
│   ├── tariff_scenarios.csv # Tariff exposure scenarios
│   ├── timeline.csv         # Manufacturing phases
├── modules/                 # Modular R scripts
│   ├── map.R                # Global operations map
│   ├── tariff.R             # Tariff scenario planner
│   ├── timeline.R           # Manufacturing phase timeline
├── www/                     # Static assets
│   ├── styles.css           # Custom styling
│   ├── pharma-logo.png      # Pharma branding logo
│   ├── us-logo.png          # U.S. strategy logo
│   ├── israel-logo.png      # Israel strategy logo
├── README.md                # This file
```


# Pharma Tariff Strategy Dashboard

This repository hosts an R Shiny application analyzing EU pharmaceutical tariff strategies, visualizing global operations, tariff exposure scenarios, and phased manufacturing rollouts. Designed for supply chain and sales professionals, it showcases how analytics—powered by tools like Qore.AI—can drive cost-saving decisions. Inspired by automotive challenges like the Chevrolet Suburban’s D&H fee surge ($995 in 2015 to $2,195 in 2025), it aligns with the mantra, “Everyone who works for me is in sales. Nothing happens until we make a sale,” turning data into sales-ready insights.

---

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Why This Matters](#why-this-matters)
- [Repository Structure](#repository-structure)
- [Setup Instructions](#setup-instructions)
- [Running the App](#running-the-app)
- [Deployment](#deployment)
- [Data Sources](#data-sources)
- [Conclusion](#conclusion)

---

## Overview

The EU imposes tariffs on pharmaceutical imports, pushing manufacturers to optimize production locations. This R Shiny app explores strategies—EU-only, Israel bridge, U.S. expansion—to cut tariff exposure from 100% to as low as 5%. With a branded launch page featuring `pharma-logo.png`, `us-logo.png`, and `israel-logo.png`, it offers:
- A global operations map (e.g., Sanofi in France, Teva in Israel).
- Tariff scenario charts comparing EU, Israel, and U.S. strategies.
- A timeline for phased rollouts (2025–2029).

For automotive sales directors eyeing Qore.AI, this mirrors analyzing D&H costs—clarity that drives sales.

---

## Key Features

1. **Global Operations Map**:
   - Interactive Leaflet map showing pharma hubs (e.g., Novartis in Switzerland, Lat 46.9481, Lon 7.4474).
   - Highlights strategic locations for tariff avoidance.

2. **Tariff Scenario Planner**:
   - Bar chart comparing exposure: EU Only (100%), Israel Bridge (50%), Full U.S. (5%).
   - Branded with `us-logo.png` to emphasize U.S. strategy.

3. **Manufacturing Phase Plan**:
   - Gantt-style timeline (2025–2029) for Israel setup to U.S. operations.
   - Features `israel-logo.png` for regional focus.

4. **Branded UI**:
   - Launch page with `pharma-logo.png`, `us-logo.png`, `israel-logo.png`.
   - Responsive design via `styles.css` for professional polish.

---

## Why This Matters

For an automotive sales director, this app isn’t just about pharma—it’s a blueprint for tackling costs like the Suburban’s 120.6% D&H hike (vs. 30.3% inflation). Here’s why it resonates, especially for Qore.AI’s analytics:

- **Sales Enablement**: Your quote—“Everyone’s in sales”—fits perfectly. Visualizing tariffs (100% to 5%) equips teams to negotiate better, just as D&H transparency could win Chevy buyers.
- **Cost Optimization**: Supply chain pros can model U.S. vs. Israel production to save millions, like optimizing GM’s logistics (fuel, wages drove D&H up).
- **Competitive Positioning**: Knowing Ford’s $2,095 D&H keeps GM competitive; this app’s global map mirrors tracking supplier networks.
- **Scalable Analytics**: Qore.AI’s low-code platform could replicate this for your dealership—e.g., D&H breakdowns in days, not weeks.
- **Future Resilience**: With 2025 tariffs looming, this app’s timeline (Israel 2025, U.S. 2028) shows proactive planning—vital for logistics volatility.

This app proves Qore.AI can turn complex data into sales wins, fast.

---

## Repository Structure

```
PharmaTariffStrategyDashboard/
├── app.R                    # Main Shiny app
├── data/                    # CSV datasets
│   ├── locations.csv        # Global pharma locations
│   ├── tariff_scenarios.csv # Tariff exposure scenarios
│   ├── timeline.csv         # Manufacturing phases
├── modules/                 # Modular R scripts
│   ├── map.R                # Global operations map
│   ├── tariff.R             # Tariff scenario planner
│   ├── timeline.R           # Manufacturing phase timeline
├── www/                     # Static assets
│   ├── styles.css           # Custom styling
│   ├── pharma-logo.png      # Pharma branding logo
│   ├── us-logo.png          # U.S. strategy logo
│   ├── israel-logo.png      # Israel strategy logo
├── README.md                # This file
```

---

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/PharmaTariffStrategyDashboard.git
   cd PharmaTariffStrategyDashboard
   ```

2. **Install R and RStudio**:
   - Download [R](https://cran.r-project.org/) and [RStudio](https://rstudio.com/products/rstudio/download/).

3. **Install Dependencies**:
   - In RStudio:
     ```R
     install.packages(c("shiny", "plotly", "leaflet", "dplyr", "bslib", "shinyjs", "readr"))
     ```

4. **Verify Files**:
   - Check structure:
     ```R
     list.files() # app.R, data/, modules/, www/
     list.files("www/") # styles.css, pharma-logo.png, us-logo.png, israel-logo.png
     ```

5. **Add Logos** (if missing):
   - Place `pharma-logo.png`, `us-logo.png`, `israel-logo.png` in `www/`.
   - Use placeholders (e.g., pharma icon, U.S./Israel flags) if needed.

---

## Running the App

1. **Set Working Directory** (optional):
   - In RStudio:
     ```R
     setwd("/path/to/PharmaTariffStrategyDashboard")
     ```

2. **Run Locally**:
   - Open `app.R` and click “Run App” or:
     ```R
     shiny::runApp()
     ```
   - Launches a launch page with three logos, title, and “Enter Dashboard” button.

3. **Interact**:
   - **Launch Page**: Shows `pharma-logo.png`, `us-logo.png`, `israel-logo.png`. Click to enter.
   - **Tabs**:
     - **Global Operations Map**: Leaflet map of pharma sites.
     - **Tariff Scenario Planner**: Bar chart with `us-logo.png`.
     - **Manufacturing Phase Plan**: Timeline with `israel-logo.png`.

---

## Deployment

To deploy on [shinyapps.io](https://www.shinyapps.io/):

1. **Install rsconnect**:
   ```R
   install.packages("rsconnect")
   ```

2. **Configure shinyapps.io**:
   - Get token/secret from [shinyapps.io dashboard](https://www.shinyapps.io/).
   - In RStudio: **Tools > Global Options > Publishing > Connect**.

3. **Deploy**:
   ```R
   library(rsconnect)
   deployApp(force = TRUE)
   ```

4. **Troubleshoot**:
   - Ensure PNGs are lowercase (`pharma-logo.png`, not `Pharma-Logo.PNG`).
   - Check logs on shinyapps.io.
   - Force re-upload if needed:
     ```R
     deployApp(force = TRUE)
     ```

---

## Data Sources

- **locations.csv**: Simulated pharma hubs (e.g., Sanofi, Lat 48.8566, Lon 2.3522).
- **tariff_scenarios.csv**: Mock tariff exposures (EU Only: 100%, Full U.S.: 5%).
- **timeline.csv**: Phased plan (Israel Setup: 2025, U.S. Ops: 2028–2029).

---

## Conclusion

This R Shiny app transforms tariff complexity into clear visuals, empowering sales and supply chain teams. For Qore.AI prospects, it’s a proof-of-concept: data drives sales, whether it’s pharma tariffs or Chevy D&H. Clone, run, and see analytics in action.



```plain
# PharmaTariffStrategyDashboard/app.R

# Load required packages
if (!require("shiny")) install.packages("shiny")
if (!require("plotly")) install.packages("plotly")
if (!require("leaflet")) install.packages("leaflet")
if (!require("dplyr")) install.packages("dplyr")
if (!require("bslib")) install.packages("bslib")
if (!require("shinyjs")) install.packages("shinyjs")
if (!require("readr")) install.packages("readr")

library(shiny)
library(plotly)
library(leaflet)
library(dplyr)
library(bslib)
library(shinyjs)
library(readr)

# Check module files
module_files <- c("modules/map.R", "modules/tariff.R", "modules/timeline.R")
for (file in module_files) {
  if (!file.exists(file)) stop(paste("Module file not found:", file))
}

# Source modules
source("modules/map.R")
source("modules/tariff.R")
source("modules/timeline.R")

# Check data files
data_files <- c("data/locations.csv", "data/tariff_scenarios.csv", "data/timeline.csv")
for (file in data_files) {
  if (!file.exists(file)) stop(paste("Data file not found:", file))
}

# Check www files (case-sensitive for deployment)
www_files <- c("www/styles.css", "www/pharma-logo.png", "www/us-logo.png", "www/israel-logo.png")
for (file in www_files) {
  if (!file.exists(file)) stop(paste("WWW file not found:", file))
}

# Load data
locations <- read_csv("data/locations.csv")
tariff_scenarios <- read_csv("data/tariff_scenarios.csv")
timeline <- read_csv("data/timeline.csv")

# UI
ui <- fluidPage(
  theme = bs_theme(
    bg = "#ffffff",
    fg = "#202124",
    primary = "#0066cc",
    base_font = font_google("Inter")
  ),
  useShinyjs(),
  tags$head(
    tags$link(rel = "icon", href = "pharma-logo.png", type = "image/png"),
    tags$link(rel = "stylesheet", type = "text/css", href = "styles.css")
  ),
  uiOutput("page")
)

# Server
server <- function(input, output, session) {
  rv <- reactiveValues(page = "launch")

  output$page <- renderUI({
    if (rv$page == "launch") {
      div(
        class = "launch-page",
        div(
          class = "logo-container",
          img(src = "pharma-logo.png", class = "launch-logo"),
          img(src = "us-logo.png", class = "launch-logo"),
          img(src = "israel-logo.png", class = "launch-logo")
        ),
        h1("EU Pharma Tariff Strategy Dashboard"),
        p("Explore manufacturing strategies to minimize EU tariff exposure. Visualize global operations, tariff scenarios, and phased rollouts for a resilient supply chain."),
        actionButton("enter_analysis", "Enter Dashboard", class = "btn-enter")
      )
    } else {
      div(
        class = "dashboard",
        titlePanel("EU Pharma Tariff Strategy Dashboard"),
        tabsetPanel(
          tabPanel("Global Operations Map", mapUI("map")),
          tabPanel("Tariff Scenario Planner", tariffUI("tariff")),
          tabPanel("Manufacturing Phase Plan", timelineUI("timeline"))
        )
      )
    }
  })

  observeEvent(input$enter_analysis, {
    rv$page <- "dashboard"
  })

  # Call module servers
  mapServer("map", locations)
  tariffServer("tariff", tariff_scenarios)
  timelineServer("timeline", timeline)
}

# Run the app
shinyApp(ui = ui, server = server)
```

```plain
# PharmaTariffStrategyDashboard/modules/map.R

mapUI <- function(id) {
  ns <- NS(id)
  tagList(
    h3("Global Operations Map"),
    p("Key pharmaceutical manufacturing locations worldwide."),
    leafletOutput(ns("map"), height = "600px")
  )
}

mapServer <- function(id, locations) {
  moduleServer(id, function(input, output, session) {
    output$map <- renderLeaflet({
      leaflet(locations) %>%
        addTiles() %>%
        addCircleMarkers(
          lng = ~Lon, lat = ~Lat,
          label = ~Company,
          radius = 6,
          color = "blue",
          fillOpacity = 0.7
        )
    })
  })
}
```

```plain
# PharmaTariffStrategyDashboard/modules/tariff.R

tariffUI <- function(id) {
  ns <- NS(id)
  tagList(
    h3("Tariff Scenario Planner"),
    img(src = "us-logo.png", class = "tab-logo"),
    p("Estimates tariff exposure based on relocation strategies (EU only, Israel bridge, or U.S. presence)."),
    plotlyOutput(ns("tariff_plot"))
  )
}

tariffServer <- function(id, tariff_scenarios) {
  moduleServer(id, function(input, output, session) {
    output$tariff_plot <- renderPlotly({
      plot_ly(tariff_scenarios, x = ~Scenario, y = ~Exposure, type = "bar",
              marker = list(color = "skyblue")) %>%
        layout(
          title = "Tariff Exposure by Manufacturing Strategy",
          xaxis = list(title = "Strategy"),
          yaxis = list(title = "Tariff Exposure (%)"),
          plot_bgcolor = "transparent",
          paper_bgcolor = "transparent"
        )
    })
  })
}
```

```plain
# PharmaTariffStrategyDashboard/modules/timeline.R

timelineUI <- function(id) {
  ns <- NS(id)
  tagList(
    h3("Manufacturing Phase Plan"),
    img(src = "israel-logo.png", class = "tab-logo"),
    p("Timeline for phased strategy: Israeli operations, then U.S. expansion."),
    plotlyOutput(ns("timeline_plot"))
  )
}

timelineServer <- function(id, timeline) {
  moduleServer(id, function(input, output, session) {
    output$timeline_plot <- renderPlotly({
      plot_ly(timeline) %>%
        add_segments(
          x = ~Start, xend = ~End, y = ~Phase, yend = ~Phase,
          line = list(color = "darkseagreen", width = 10),
          text = ~paste(Phase, "<br>", Start, " to ", End),
          hoverinfo = "text"
        ) %>%
        layout(
          title = "Phased Manufacturing Rollout",
          xaxis = list(title = "Timeline", type = "date"),
          yaxis = list(title = "Phase", autorange = "reversed"),
          plot_bgcolor = "transparent",
          paper_bgcolor = "transparent",
          showlegend = FALSE
        )
    })
  })
}
```

```plain
/* PharmaTariffStrategyDashboard/www/styles.css */
.launch-page {
  text-align: center;
  padding: 50px;
  background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://images.unsplash.com/photo-1505751172876-fa1923c5c282') no-repeat center;
  background-size: cover;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  color: #ffffff;
}
.launch-page h1 {
  font-size: 2.5em;
  margin-bottom: 20px;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
}
.launch-page p {
  font-size: 1.1em;
  max-width: 600px;
  margin: 0 auto 30px;
}
.launch-page .btn-enter {
  font-size: 1.2em;
  padding: 10px 20px;
  background-color: #0066cc;
  color: #ffffff;
  border: none;
  border-radius: 20px;
  cursor: pointer;
  transition: background-color 0.3s;
}
.launch-page .btn-enter:hover {
  background-color: #004c99;
}
.logo-container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  gap: 20px;
  margin-bottom: 20px;
}
.launch-logo {
  width: 100px;
  height: auto;
}
.tab-logo {
  width: 100px;
  margin-bottom: 10px;
}
.dashboard {
  padding: 20px;
}
body {
  font-family: 'Inter', sans-serif;
}
h3 {
  color: #0066cc;
}
p {
  color: #202124;
  margin-bottom: 20px;
}
```

```plain
Company,Country,Lat,Lon
Sanofi,France,48.8566,2.3522
Novartis,Switzerland,46.9481,7.4474
Takeda,Japan,35.6895,139.6917
Astellas,Japan,35.4437,139.6380
Bayer,Germany,52.5200,13.4050
Novo Nordisk,Denmark,55.6761,12.5683
Teva,Israel,32.0853,34.7818
```

```plain
Scenario,Exposure
EU Only,100
EU + Israel,70
Israel Bridge,50
Israel + US,25
Full US Manufacturing,5
```

<xaiArtifact artifact_id="ddf8c983-9fd6-4952-bd67-cc0a5ca7efcd" artifact_version_id="93498605-d220-4465-881f-ae80bc421de6" title="timeline.csv" contentType="text/plain">
Phase,Start,End
Israel Setup,2025-01-01,2025-12-31
Israel Ramping,2026-01-01,2026-06-01
US Site Selection,2026-06-01,2026-12-31
US Buildout,2027-01-01,2027-12-31
US Full Ops,2028-01-01,2029-01-01
</xaiArtifact>

### Notes for GitHub Setup

1. **Create the Repository**:
   - Go to [GitHub](https://github.com/) and sign in.
   - Click **New** repository.
   - Name: `PharmaTariffStrategyDashboard`.
   - Description: “R Shiny app visualizing EU pharma tariff strategies for supply chain and sales insights.”
   - Set to **Public** (or Private).
   - Initialize with a README (optional; replace with above `README.md`).

2. **Push the Code**:
   - Locally:
     ```bash
     git init
     git add .
     git commit -m "Initial commit: Pharma tariff strategy dashboard"
     git remote add origin https://github.com/your-username/PharmaTariffStrategyDashboard.git
     git push -u origin main
     ```
   - Or use GitHub Desktop/RStudio’s Git pane.

3. **Add Logos**:
   - Ensure `www/pharma-logo.png`, `www/us-logo.png`, `www/israel-logo.png` are included.
   - If missing, download placeholders (e.g., pharma icon, U.S./Israel flags) and rename exactly (lowercase).
   - Commit:
     ```bash
     git add www/pharma-logo.png www/us-logo.png www/israel-logo.png
     git commit -m "Add logo files"
     git push
     ```

4. **Verify Deployment**:
   - Deploy to shinyapps.io:
     ```R
     library(rsconnect)
     deployApp(force = TRUE)
     ```
   - Update `README.md` with the URL (e.g., `https://your-account.shinyapps.io/PharmaTariffStrategyDashboard/`).

5. **Polish the Repo**:
   - Add `.gitignore`:
     ```
     .Rhistory
     .RData
     .Rproj.user/
     *.Rproj
     ```
   - Commit:
     ```bash
     git add .gitignore
     git commit -m "Add .gitignore"
     git push
     ```

### Deployment Notes

- **Case-Sensitivity**: All PNGs (`pharma-logo.png`, `us-logo.png`, `israel-logo.png`) are lowercase to avoid errors like `chevy-logo.png`.
- **Troubleshooting**:
  - If logos fail to load:
    ```R
    list.files("www/") # Verify files
    deployApp(force = TRUE)
    ```
  - Check shinyapps.io logs.

### Why This Matters (Excerpt from README)

> For an automotive sales director, this app isn’t just about pharma—it’s a blueprint for tackling costs like the Suburban’s 120.6% D&H hike (vs. 30.3% inflation). Here’s why it resonates, especially for Qore.AI’s analytics:
> - **Sales Enablement**: Your quote—“Everyone’s in sales”—fits perfectly. Visualizing tariffs (100% to 5%) equips teams to negotiate better, just as D&H transparency could win Chevy buyers.
> - **Cost Optimization**: Supply chain pros can model U.S. vs. Israel production to save millions, like optimizing GM’s logistics (fuel, wages drove D&H up).
> - **Competitive Positioning**: Knowing Ford’s $2,095 D&H keeps GM competitive; this app’s global map mirrors tracking supplier networks.
> - **Scalable Analytics**: Qore.AI’s low-code platform could replicate this for your dealership—e.g., D&H breakdowns in days, not weeks.
> - **Future Resilience**: With 2025 tariffs looming, this app’s timeline (Israel 2025, U.S. 2028) shows proactive planning—vital for logistics volatility.

Please review the repository details and let me know if you’re happy with it. If you approve, I’ll draft the LinkedIn post. If you want tweaks (e.g., more details, different phrasing), let me know what to adjust!
