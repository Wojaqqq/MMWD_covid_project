# MMWD_covid_project

The issue relates to solving the problem of getting food to people who are in home quarantine. Each restaurant has a list of the homes it can serve, as well as the 
the number of meals available. The number of residents in each home determines the demand for meals and is served by one company/can be served by 
multiple companies. An additional parameter is the distance of the houses from the restaurant. We want to minimise the sum of the distances between the restaurants and the homes they serve 
taking into account the capacity of the catering establishments. We will realise this using an evolutionary algorithm.


Project carried out in a team of 3: Balbina Molerus, Tomasz Wojakowski, Bartosz Nieroda.

**Input data:**

List of restaurants with information:
  - possible delivery range 
  - number of servings per day

List of houses with information:
  - location
  - meal requirements (portions) 

**Assumptions:**

  - the house receives the entire demand from one restaurant or can accept split portions from several.
  - the daily restaurant throughput is constant
  - the daily demand of the houses is constant
  - we assume that after each delivery, the supplier returns to the dwelling for further portions
  - there is one route between the dwelling and the restaurant 


**Mathematical model:**

Parameters:
  - R - collection of restaurants serving meals
  - M - set of flats with people in quarantine
  - Di,j - the path separating the restaurants and the flats
  - Pi - meal portion requirement for each flat in quarantine
  - Ji - number of possible meal portions delivered by the restaurant

Objective function

![image](https://user-images.githubusercontent.com/49729749/111630480-b2691a80-87f2-11eb-82cd-6f33e918f1c7.png)


