# Predicting Future Frequency of Disasters by State

### Description
Natural disasters are costly events that can have financial impacts outside cleanup efforts. When financial aid for natural disasters is under-provisioned, this proves to be a potential risk of 7.25 billion dollars per disaster outside the predicted count. When natural disaster funds are over-provisioned, this means fewer funds going towards initiatives to better the lives of citizens (schools, roads, large-scale state & federal projects), ultimately resulting in an opportunity cost more significant than the natural disaster.  

This model aims to provide a better estimate of natural disasters by the state for the upcoming calendar year. In 2021 alone, natural disasters cost the United States a total of [145 billion dollars](https://www.climate.gov/news-features/blogs/beyond-data/2021-us-billion-dollar-weather-and-climate-disasters-historical), with there being 20 FEMA-declared natural disasters in the calendar year, meaning on average a natural disaster costs 7.25 billion dollars. Given this figure, the potential market value of this model is between 75,000,000 to 82,500,000 dollars, should the model reach 50% accuracy. 


### Confusion Matrix

|                                          | Predicted: More disaster for given state | Predicted: Less disaster for given state |
| ---------------------------------------- | ---------------------------------------- | ---------------------------------------- |
| Actual: More disaster for given state    | True Positive                            | False Negative                           |
| Actual: Less disaster for given state    | False Positive                           | True Negative                            |


- Value of a true positive: true positive denotes that the ruling body was able to plan appropriately and dog-ear funds for relief, a savings of `(x)7_500_000`.
- Value of a false positive: false positive denotes that the ruling body will mismanage funds. Funds could be diverted to an appropriate initiative by the end of the fiscal year; however, it is unlikely that the total value initially dog-eared for disaster relief will be used in the given calendar year, a potential liability of `x(7_500_000 * 0.33)`.
- Value of a false negative: false negatives are more devastating than false positives, because now the funds have been allocated to other initiatives, and the given governing body will still need to pay for disaster relief, this is a liability of `(x)7_500_000`.   
- Value of a true negative: this is the best case scenario, the model predicted fewer disasters and funds were able to be diverted from disaster relief to other initiatives. Since a municipality may be able to divert funds to business development or schools there is a net gain larger than the cost of a single disaster, a savings of `x(7_500_00 * 1.1)`
