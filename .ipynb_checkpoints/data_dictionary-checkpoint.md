|Feature|Full Name|Type|Dataset|Description|
|-|-|-|-|-|
|Date|Game Date|object|n/a|The date on which the game was played.|
|Name|Player Name|object|n/a|First and last name of the player.|
|Tm|Player’s Team|object|n/a|Name of the player’s team.|
|G  |Games Played|int|standard|Number of games in which the player has appeared.|
|AB |At Bats|int|standard|Number of trips to the plate in which the batter does not walk, get hit by a pitch, sacrifice (fly or bunt), or reach on interference.|
|PA |Plate Appearances|int|standard|Number of times the player has come to the plate.|
|H  |Hits|int|standard|Number of hits.|
|1B |Singles|int|standard|Number of singles.|
|2B |Doubles|int|standard|Number of doubles.|
|3B |Triples|int|standard|Number of triples.|
|HR |Home Runs|int|standard|Number of home runs.|
|R  |Runs Scored|int|standard|Number of runs scored.|
|RBI|Runs Batted In|int|standard|Number of times a run scores as a result of a batter’s plate appearance, not counting situations in which an error caused the run to score or the batter hit into a double play.|
|BB |Walks|int|standard|Total number of walks (includes IBB).|
|IBB|Intentional Walks|int|standard|Number of times the batter was intentionally walked.|
|SO |Strikeouts|int|standard|Number of strikeouts.|
|HBP|Hit By Pitches|int|standard|Number of times the batter reached after being hit by a pitch.|
|SF |Sacrifice Flies|int|standard|Number of times a batter’s fly out allowed a runner to tag up and score.|
|SH |Sacrifice Bunts|int|standard|Any bunt in which there was a runner on base and less than two outs in which the batter was put out and at least one runner advanced.|
|GDP|Grounded into Double Play|int|standard|Number of times the batter hit into a double play.|
|SB |Stolen Bases|int|standard|Number of stolen bases.|
|CS |Caught Stealing|int|standard|Number of times caught stealing.|
|AVG|Batting Average|float|standard|Rate of hits per at bat, calculated as H/AB.|
|playerId|n/a|int|n/a|Unique identifying number for each player.|
|BB% |Walk Percentage|float|advanced| Frequency with which the batter has walked, calculated as walks divided by plate appearances.|
|K% |Strikeout Percentage|float|advanced| Frequency with which the batter has struck out, calculated as strikeouts divided by plate appearances.|
|BB/K |Walk to Strikeout Rate|float|advanced| Ratio of walks to strikeouts, calculated as Walks/Strikeouts.|
|OBP |On Base Percentage|float|advanced| Rate at which the batter reaches base, calculated as (H+BB+HBP)/(AB+BB+HBP+SF).|
|SLG |Slugging Percentage|float|advanced| Average number of total bases per at bat, calculated as Total Bases/AB.|
|OPS |On Base Plus Slugging|float|advanced| Combination of OBP and SLG, calculated as OBP+SLG.|
|ISO |Isolated Power|float|advanced| Average number of extra bases per at bat, calculated several ways such as SLG minus AVG.|
|BABIP |Batting Average on Balls in Play|float|advanced| The rate at which the batter gets a hit when he puts the ball in play, calculated as (H-HR)/(AB-K-HR+SF).|
|wRC |Weighted Runs Created|float|advanced| Number of runs a player has generated for his team as a result of his wOBA and playing time.|
|wRAA |Weighted Runs Above Average|float|advanced| Number of runs above or below average a player has added as a hitter.|
|wOBA |Weighted On Base Average|float|advanced| Combines all the different aspects of hitting into one metric, weighting each of them in proportion to their actual run value. While batting average, on-base percentage, and slugging percentage fall short in accuracy and scope, wOBA measures and captures offensive value more accurately and comprehensively.|
|wRC+ |Weighted Runs Created Plus|float|advanced| The most comprehensive rate statistic used to measure hitting performance because it takes into account the varying weights of each offensive action (like wOBA) and then adjusts them for the park and league context in which they took place.|
|GB/FB|Ground Ball to Fly Ball Ratio|float|batted ball|The ratio of ground balls a batter hits to fly balls, calculated as GB/FB.|
|LD%  |Line Drive Percentage|float|batted ball|The percentage of a batter’s balls in play that are line drives, calculated as LD/BIP.|
|GB%  |Ground Ball Percentage|float|batted ball|The percentage of a batter’s balls in play that are ground balls, calculated as GB/BIP.|
|FB%  |Fly Ball Percentage|float|batted ball|The percentage of a batter’s balls in play that are fly balls, calculated as FB/BIP.|
|IFFB%|Infield Fly Ball Percentage|float|batted ball|Percentage of a batter’s fly balls that were infield fly balls, calculated as IFFB/FB.|
|HR/FB|Home Run to Fly Ball Rate|float|batted ball|Percentage of a batter’s fly balls that go for home runs, calculated as HB/FB (even though some HR are line drives).|
|IFH% |Infield Hit Percentage|float|batted ball|Percentage of ground balls that are infield hits, calculated as IFH/GB.|
|BUH% |Bunt Hit Percentage|float|batted ball|Percentage of bunts that go for hits, calculated as Bunt Hits/Bunts.|
|Pull%|Pull Percentage|float|batted ball|Percentage of batted balls hit to the pull field.|
|Cent%|Center Percentage|float|batted ball|Percentage of batted balls hit to the middle of the field.|
|Oppo%|Opposite Field Percentage|float|batted ball|Percentage of batted balls hit to the opposite field.|
|Soft%|Soft Contact Percentage|float|batted ball|Percentage of soft-hit batted balls.|
|Med% |Medium Contact Percentage|float|batted ball|Percentage of medium-hit batted balls.|
|Hard%|Hard Contact Percentage|float|batted ball|Percentage of hard-hit batted balls.|
|prev3_pa|n/a|float|custom|Player’s rolling three-day sum number of plate appearances.|
|prev5_pa|n/a|float|custom|Player’s rolling five-day sum number of plate appearances.|
|prev3_bippa|n/a|float|custom|Player’s rolling three-day sum number of plate appearances that resulted in a ball in play (no walks or strikeouts) divided by his total number of plate appearances in that span.|
|prev5_bippa|n/a|float|custom|Player’s rolling five-day sum number of plate appearances that resulted in a ball in play (no walks or strikeouts) divided by his total number of plate appearances in that span.|
|hpa|n/a|float|custom|Player’s number of hits divided by his number of plate appearances in that day’s game.|
|prev3_hpa|n/a|float|custom|Player’s rolling three-day sum number of hits divided by his number of plate appearances in that span.|
|prev5_hpa|n/a|float|custom|Player’s rolling five-day sum number of hits divided by his number of plate appearances in that span.|
|next_game_hit|n/a|bool|custom|A binary indicator of whether or not the player will record a hit in his next game. Used as the target y variable.|