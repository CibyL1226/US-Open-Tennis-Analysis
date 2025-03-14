# milestone2 - Investigating Tennis Court Material's Affect on Player Performance

link to original dataset: https://github.com/JeffSackmann/tennis_atp

Report slide deck: scratching_the_sruface PDF

tourney_id
- a unique identifier for each tournament, such as 2020-888. The exact formats are borrowed from several different sources, so while the first four characters are always the year, the rest of the ID doesn't follow a predictable structure.

tourney_name
surface
draw_size
- number of players in the draw, often rounded up to the nearest power of 2. (For instance, a tournament with 28 players may be shown as 32.)

tourney_level
- For men: 'G' = Grand Slams, 'M' = Masters 1000s, 'A' = other tour-level events, 'C' = Challengers, 'S' = Satellites/ITFs, 'F' = Tour finals and other season-ending events, and 'D' = Davis Cup 
- For women, there are several additional tourney_level codes, including 'P' = Premier, 'PM' = Premier Mandatory, and 'I' = International. The various levels of ITFs are given by the prize money (in thousands), such as '15' = ITF $15,000. Other codes, such as 'T1' for Tier I (and so on) are used for older WTA tournament designations. 'D' is used for Federation/Fed/Billie Jean King Cup, and also for Wightman Cup and Bonne Bell Cup.

- Others, eventually for both genders: 'E' = exhibition (events not sanctioned by the tour, though the definitions can be ambiguous), 'J' = juniors, and 'T' = team tennis, which does yet appear anywhere in the dataset but will at some point.

tourney_date
- eight digits, YYYYMMDD, usually the Monday of the tournament week.

match_num
- a match-specific identifier. Often starting from 1, sometimes counting down from 300, and sometimes arbitrary. 

winner_id
- the player_id used in this repo for the winner of the match

winner_seed
winner_entry
- 'WC' = wild card, 'Q' = qualifier, 'LL' = lucky loser, 'PR' = protected ranking, 'ITF' = ITF entry, and there are a few others that are occasionally used.

winner_name
winner_hand
- R = right, L = left, U = unknown. For ambidextrous players, this is their serving hand.
winner_ht
- height in centimeters, where available

winner_ioc
- three-character country code

winner_age
- age, in years, as of the tourney_date

loser_id
loser_seed
loser_entry
loser_name
loser_hand
loser_ht
loser_ioc
loser_age
score
best_of
- '3' or '5', indicating the the number of sets for this match

round
minutes
- match length, where available

w_ace
- winner's number of aces
w_df
- winner's number of doubles faults
w_svpt
- winner's number of serve points
w_1stIn
- winner's number of first serves made
w_1stWon
- winner's number of first-serve points won
w_2ndWon
- winner's number of second-serve points won
w_SvGms
- winner's number of serve games
w_bpSaved
- winner's number of break points saved
w_bpFaced
- winner's number of break points faced

l_ace
l_df
l_svpt
l_1stIn
l_1stWon
l_2ndWon
l_SvGms
l_bpSaved
l_bpFaced

winner_rank
- winner's ATP or WTA rank, as of the tourney_date, or the most recent ranking date before the tourney_date
winner_rank_points
- number of ranking points, where available
loser_rank
loser_rank_points
