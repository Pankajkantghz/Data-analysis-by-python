# Tampa Bay Rays Pitching Analysis

## Overview
This SQL analysis explores various aspects of Tampa Bay Rays pitching performance using two primary tables:
- `RaysPitching.Dbo.LastPitchRays`
- `RaysPitching.Dbo.RaysPitchingStats`

## Analysis Sections

### 1. Pitches Per At-Bat Analysis
- Average pitches per at-bat
- Home vs. Away performance
- Lefty vs. Righty batter analysis
- Pitcher-specific pitch counts
- Most common pitch sequences

### 2. Last Pitch Analysis
- Frequency of last pitches thrown
- Fastball vs. Offspeed pitch distribution
- Comparison between Relief and Starting Pitchers

### 3. Home Run Analysis
- Pitches most likely to result in home runs
- Home run distribution by pitch zone
- Home run patterns by count and pitcher type

### 4. Shane McClanahan Specific Analysis
- Detailed performance metrics
- Pitch effectiveness by infield position
- Pitch performance with runners on base
- Lowest launch speed pitches

## Key SQL Techniques Used
- Window Functions
- Partition By
- Common Table Expressions (CTEs)
- Union Queries
- Ranking
- Aggregation Functions
- Case Statements

## Requirements
- Microsoft SQL Server
- Access to RaysPitching database

## Potential Insights
- Pitch strategy optimization
- Pitcher performance evaluation
- Situational pitching effectiveness

## Limitations
- Data dependent on specific dataset
- Some queries may require data cleaning

## Sample Queries

### Average Pitches Per At-Bat
```sql
SELECT AVG(1.00 * Pitch_number) AvgNumofPitchesPerAtBat
FROM RaysPitching.Dbo.LastPitchRays
