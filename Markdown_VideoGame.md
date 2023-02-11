# Video Games Rating By 'ESRB'

**Video games** have many ratings, here we do 
*machine learning* to predict the rating of 
the game according to the available data.


## Team members
| Team members      | Role                                                     |
|-------------------|----------------------------------------------------------|
| Sulaiman (Leader) | EDA, Charts, support of ML and Comparison of two models. |
| Razan Fahad       | Charts and ML Random forest.                             |
| Waleed Almutairi  | Charts  , ML DecisionTreeClassifier and Markdown.        |


## Dataset Overview:
This data contains the name for 1895 games with 34 of ESRB rating content 
with the name and console as features for each game.

A single data point is represented as a binary value 0-1 for 
Console and a binary vector for the features of ESRB content.

**Note:** (0 = PS4)  (1 = PS4 & Xbox_one)

[Dataset](https://www.kaggle.com/datasets/imohtn/video-games-rating-by-esrb)


## Dataset Description:
| Column                   | Description                                                                                                                                                         |
|--------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| title                    | Name of the game.                                                                                                                                                   |
| console                  | The console on which the game was released.                                                                                                                         |
| Alcohol_Reference        | Reference to and/or images of alcoholic beverages.                                                                                                                  |
| Animated_Blood           | Discolored and/or unrealistic depictions of blood.                                                                                                                  |
| Blood                    | Depictions of blood.                                                                                                                                                |
| Blood_and_Gore           | Depictions of blood or the mutilation of body parts.                                                                                                                |
| Cartoon_Violence         | Violent actions involving cartoon-like situations and characters. May include violence where a character is unharmed after the action has been inflicted.           |
| Crude_Humor              | Depictions or dialogue involving vulgar antics, including "bathroom" humor.                                                                                         |
| DrugRe_ference           | Reference to and/or images of illegal drugs.                                                                                                                        |
| Fantasy_Violence         | Violent actions of a fantasy nature, involving human or non-human characters in situations easily distinguishable from real life.                                   |
| Intense_Violence         | Graphic and realistic-looking depictions of physical conflict. May involve extreme and/or realistic blood, gore, weapons, and depictions of human injury and death. |
| Language 	               | Moderate use of profanity.                                                                                                                                          |
| Lyrics                   | References to profanity, sexuality, violence, alcohol, or drug use in music.                                                                                        |
| Mature_Humor             | Depictions or dialogue involving "adult" humor, including sexual references.                                                                                        |
| Mild_Blood               | Some blood.                                                                                                                                                         |
| Mild_Cartoon_Violence    | Some violent actions involving cartoon.                                                                                                                             |
| Mild_Fantasy_Violence    | Some violent actions of a fantasy nature.                                                                                                                           |
| Mild_Language            | Mild to moderate use of profanity.                                                                                                                                  |
| Mild_Lyrics              | Mild References to profanity, sexuality, violence, alcohol, or drug use in music.                                                                                   |
| Mild_Suggestive_Themes   | some provocative references or materials.                                                                                                                           |
| Mild_Violence            | Some scenes involving aggressive conflict.                                                                                                                          |
| No_Descriptors           | No content descriptors.                                                                                                                                             |
| Nudity                   | Graphic or prolonged depictions of nudity.                                                                                                                          |
| Partial_Nudity  	        | Brief and/or mild depictions of nudity.                                                                                                                             |
| Sexual_Content           | Non-explicit depictions of sexual behavior, possibly including partial nudity.                                                                                      |
| Sexual_Themes            | References to sex or sexuality.                                                                                                                                     |
| Simulated_Gambling       | Player can gamble without betting or wagering real cash or currency.                                                                                                |
| Strong_Language          | Explicit and/or frequent use of profanity.                                                                                                                          |
| Strong_Sexual_Content    | Explicit and/or frequent depictions of sexual behavior, possibly including nudity.                                                                                  |
| Suggestive_Themes        | Provocative references or materials.                                                                                                                                |
| Use_of_Alcohol           | The consumption of alcoholic beverages.                                                                                                                             |
| Use_of_Drugs_and_Alcohol | The consumption of alcoholic and drugs beverages.                                                                                                                   |
| Violence                 | Scenes involving aggressive conflict. May contain bloodless dismemberment.                                                                                          |
| ESRB_rating              | rating: RP - EC - E - E+10 - T - M - A                                                                                                                              |

## ESRB rating description:
| ESRB_rating | Description     |
|-------------|-----------------|
| RP          | Rating Pending  |
| EC          | Early Childhood |
| E           | Everyone        |
| E 10+       | Everyone 10+    |
| T           | Teen            |
| M           | Mature          |
| A           | Adult           |

## Final results of ML models.

| Algorithms    | Time(s)            | Accuracy(%)        |
|---------------|--------------------|--------------------|
| Decision Tree | Faster (0.01-0.05) | Lower (85%-90%)    |
| Random Forest | Slower (0.70-0.80) | Higher (80%-83%)   |

