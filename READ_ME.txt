FIFA 20 Dataset Analysis


- Our Aim
    1) Present a brief data analysis for some features in FIFA 2020.
    2) Building model that Classifying playes based on Premier League Clubs.
    
    
- DataSet
    Dataset is FIFA 20
    The dataset includes the players data for the Career Mode FIFA 20. Data has been scraped from the publicly 
    available website https://sofifa.com , and  you can get this data from https://kaggle.com .
    It contains 18,278 players with 104 different attributes.
    every player in FIFA 20 has:
    - URL of the scraped player
    - Player positions, with the role in the club and in the national team
    - Player attributes with statistics as Attacking, Skills, Defense, Mentality, GK Skills, etc.
    - Player personal data like Nationality, Club, DateOfBirth, Wage, Salary, etc.
    


- Some ideas in our analysis

    1) Univariate Exploration
            Distributed of some numerical attributes.
            Count of players by age.
            Count of players by nationality.
            Count of players by preferred foot.
            Count of players by BMI(Body Mass Index).
            Players have the max values in some feature(overall ,age, potential,etc..).
            Clubs have top 20 players with a high overall.
            Nationality have top 20 players with a high overall.
            Age has Max players in Top 20.
            Proportion of Player's per Position.
            
    2) Bivariate Exploration
            Does increasing of overall rating depend on age?
            Does increasing in overall depend on BMI?
            Relation between height and weight.
            Relation between weight and pace.
            
    3) Multivariate Exploration
            Relation between Overall Rating , Value in Euros and Age.
            Relation between overall , potential and age.
            Correlation between features.
            Comparison between (MESSI VS RONALDO).
            Comparison between (M.Salah VS RONALDO).
            Comparison between (MESSI VS M.Salah)




- Summary of Findings

     - find that there is high correlation between:
            1) Wage and value
            2) release clause and value
            3) release clause and age positive correlation between:
            4) overall and potentail, weight and height, defending and physical.
            5) sprint speed and movement balance, sprint speed and ball control, sprint speed and pace.
            6) shooting and dribbling, shooting and attacking finishing.

     - The result of exploration
            1) Distributions for in value_eur wage_eur and release_clause_eur are highly skewed to the right.
            2) We can say that distribution for overall and potential is normal.
            3) There are many outliers in value & wage & release clause and pace, Few outliers in overall & weight and height 
            and potential.
            4) L.Messi is the most player has high overall & wage & release_clause & attacking_finishing & dribbling & 
            mentality_vision .
            5) Neymar Jr has high value.
            6)Cristiano Ronaldo has high power_shot.
            7) C. Muñoz is the oldest player with 42 years old.
            8) V. van Dijk has high defending.
            9) Age doesn't linearly effect overall rating, Maximum of rating first increases and then decreases.
            10) Height and weight, show that Height and weight are linearly dependant
            11) Pace and weight, Pace tends to decrease with increase in weight.
            12) Height and defending, show that the highest defending has the height between 180-190 with few outliers compared 
            to the lowest defending.
            13) There is no direct relation between BMI and overall, because there are outliers effect on the relation, Maximum 
            of rating increases and then decreases.
            14) Overall rating & Value and age, players with highest overall rating are valued more based on age group 25-30.
            15) Overall rating & potential and age, There is linearly dependant relation between Overall Rating and Potential, 
            we can see that the younger players have the highest potential.
            16) RadarChart display that Messi is better than Ronaldo in dribbling & passing & overall & defending & potential.
            17) Ronaldo is better than Messi in physical & shooting & pace.
            18) M.Salah is better than Messi in defending & physical & pace.
            19) Messi is better than M.Salah in dribbling & passing & overall & shooting & potential.
            20) M.Salah is better than Ronaldo in defending & pace.
            21) Ronaldo is better than M.Salah in passing & overall & shooting & potential & physical .

    - The result of hypothesis test
            1) Preferred foot doesn't have a significant impact on the overall score.
            2) Preferred foot have a significant impact on the attacking finishing.
            
    - The result of models
            Random Forest Classifier (RFC) Model has the highest accuracy with 69% ,The next is Support Vector Machine (SVM) 
            with accuracy 65%, and Decision Tree with accuracy 60% ,and KKN Cluster with accuracy 57%.
            
- Limitations of data
    The market value of the clubs.
    