# 🎬 Cinema Audience Forecasting Challenge

Time-series forecasting project focused on predicting daily cinema audience attendance using multi-source booking data.

---

##  Overview

This competition presents a real-world time-series forecasting problem centered on predicting **daily theatre audience counts**.

The dataset integrates booking and attendance data from two independent systems:

- **BookNow** – Online ticket booking and aggregation platform.
- **CinePOS** – Theatre-installed Point-of-Sale (POS) ticketing system.

Participants must leverage historical booking patterns, theatre attributes, and calendar features to forecast future audience attendance.

---

##  Objective

Predict:

For each:

As specified in `sample_submission.csv`.

---

## 📂 Dataset Description

The dataset contains **8 CSV files** (~102 MB total) including historical bookings, theatre metadata, audience visits, and calendar information.

### 📁 Files Included

| File Name | Description |
|------------|-------------|
| `cinePOS_theaters.csv` | Theatre metadata from CinePOS system |
| `booknow_theaters.csv` | Theatre metadata from BookNow platform |
| `movie_theater_id_relation.csv` | Mapping between BookNow and CinePOS theatre IDs |
| `cinePOS_booking.csv` | On-site POS ticket sales |
| `booknow_booking.csv` | Online advance bookings |
| `booknow_visits.csv` | Daily recorded audience counts |
| `date_info.csv` | Calendar features (holidays, weekdays, etc.) |
| `sample_submission.csv` | Submission format template |

---

##  Data Characteristics

- 27 columns
- Time-series structured data
- Anonymized dataset
- Latitude & longitude are approximate
- Some theatres may be closed on certain days
- Zero audience days are included but ignored in final scoring

---

##  Key Forecasting Considerations

Audience counts may be influenced by:

- Holidays  
- Weekends  
- Theatre type  
- Online booking trends  
- POS booking behavior  
- Historical attendance patterns  

A strong model should:

- Combine both online and POS booking signals
- Incorporate seasonality and calendar effects
- Handle zero and missing values properly
- Capture weekly and holiday trends

---
