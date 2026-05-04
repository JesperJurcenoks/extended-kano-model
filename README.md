# Functionality Prioritization \- Stream Train \- Kano model

## When Bug fixes before Features \- break

By Jesper Jurcenoks

<sub>© Jesper Jurcenoks. Licensed under [CC-BY-4.0](LICENSE). Originally developed across netVigilance and Alert Logic; documentation first published 2026.</sub>

[**Fixing Bug vs Building Feature Prioritization	1**](#fixing-bug-vs-building-feature-prioritization)

[**1 Security Functionality (Basic Requirement a)	3**](#1-security-functionality-\(basic-requirement-a\))

[**2 Core Functionality (Basic Requirement b)	5**](#2-core-functionality-\(basic-requirement-b\))

[**3 Auxiliary Functionality (Basic Requirement c)	7**](#3-auxiliary-functionality-\(basic-requirement-c\))

[**4 Performance functionality	9**](#4-performance-functionality)

[**5 Bells and Whistles functionality	11**](#5-bells-and-whistles-functionality)

[**6 Less is more functionality (and more is worse)	13**](#6-less-is-more-functionality-\(and-more-is-worse\))

[**7 Me too/checkbox functionality	15**](#7-me-too/checkbox-functionality)

[**8 Nice to have functionality	17**](#8-nice-to-have-functionality)

[**9 Single customer functionality	18**](#9-single-customer-functionality)

[**10 Show Horse functionality	20**](#10-show-horse-functionality)

[**Behind the Scenes functionality (Honorable Mention)	22**](#behind-the-scenes-functionality-\(honorable-mention\))

[**Functionality changes over time	23**](#functionality-changes-over-time)

[Cool new Feature life cycle.	23](#cool-new-feature-life-cycle.)

[Competitor's Show Horse Life Cycle.	24](#competitor's-show-horse-life-cycle.)

We have a prioritized list of functionality.   
Within Features we will build higher priority features before lower priority features.  
And within bugs we will fix higher priority bugs before lower priority features.

We have 2 motions: 

1. Fulfill the promise we made to the market. (bugs in functionality or gap between promised features and actual features.)  
2. Expand the promise to the market (new Features)

# Fixing Bug vs Building Feature Prioritization {#fixing-bug-vs-building-feature-prioritization}

| Feature vs Bugs? | Basic Fea. bug | Perform. Bug | Bells & Whistle Bug | Less is more bugs | Me too Func bugs | Nice to have bugs | Single Cust. Bugs |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| Basic Feature | Bugs before Features | Judgement Call | Feature before Bugs | Feature before Bugs | Feature before Bugs | Feature before Bugs | Feature before Bugs |
| Performance feature | Bugs before Features | Bugs before Features | Judgement Call | Feature before Bugs | Feature before Bugs | Feature before Bugs | Feature before Bugs |
| Bells & Whistles Feature | Bugs before Features | Bugs before Features | Bugs before Features | Judgement Call | Feature before Bugs | Feature before Bugs | Feature before Bugs |
| Less is more Feature | Bugs before Features | Bugs before Features | Bugs before Features | Bugs before Features | Judgement Call | Feature before Bugs | Feature before Bugs |
| Me too Feature | Bugs before Features | Bugs before Features | Bugs before Features | Bugs before Features | Bugs before Features | Judgement Call | Feature before Bugs |
| Nice to have Feature | Bugs before Features | Bugs before Features | Bugs before Features | Bugs before Features | Bugs before Features | Bugs before Features | Judgement Call |
| Single Cust. Feature | Bugs before Features | Bugs before Features | Bugs before Features | Bugs before Features | Bugs before Features | Bugs before Features | Bugs before Features |

# 1 Security Functionality (Basic Requirement a) {#1-security-functionality-(basic-requirement-a)}

![][image1]**Description:** Security is more important than anything. If we can build Core functionality but cannot make it secure then we should **not** build Core functionality and should exit this market. 

As a security conscious company there is even more goodwill tied to this than for other companies \- if the security model breaks down, for high severity issues in Security functionality we would be forced to disable core functionality until the high severity issue has  
been corrected.

**Customer perception of need:** for the customer this is so obvious that he need never mention it unprompted unless they had a recent bad experience. They will typically not look for this functionality in a datasheet.

**On a Steam train:** Ensure that the boiler doesn't explode and take out a city block, make sure we can brake once we get going.

**Metric:** not much to measure for here: there shouldn't be degrees of secure: Measure for abnormal behavior

**QA/QE:** This part has more unit-tests per line of code than any of the other levels. 100% of use and corner cases are covered with unit-tests. Security Review in every phase of development from Design to "push to production".  
Security testing is ongoing in the production environment.

**Kano Model:** Must-Be Quality, This is a threshold attribute, unless the product meets the threshold in this area it will soon die due to dissatisfaction. Examples: a Milk carton's ability to not leak. As long as it does not leak, nobody cares about the ability to hold milk. Once it leaks customers become extremely dissatisfied.

![][image2]  
Functionality vs Satisfaction: Rarely will higher security functionality improve the customer satisfaction, it needs to be there, it needs to work and that’s it, not working and satisfaction drops very fast. 

# 2 Core Functionality (Basic Requirement b)  {#2-core-functionality-(basic-requirement-b)}

![][image3]**Description:** Without this we have no reason to be in this business, this is why the customers buy this product, if this breaks then all customer value is gone. We should do this extremely well. Core Functionality includes the primitives that allows customers to create workarounds for their special needs. 

**Customer perception of need:** for the customer this is so obvious that he need never mention it unprompted unless he had a recent bad experience. He will typically not look for this functionality in a datasheet. Customers will easily be able to see if we cannot do this, it will be painfully obvious if we cannot do this at all during a Demo or Proof of Concept. However the customer will have a hard time judging how well we do this until he has used the product for a while. 

**On a Steam train:** the Ability to haul a load forward. Without this ability- what is the point? Make sure we can haul more than just the resources (wood, coals, water) we are consuming. 

**In a hotel:** The Non-smoking rooms

**Metric:** Measure customer value, this is where we measure if we are delivering on our basic customer promise. There are 2 thresholds for this metric: 1\) As long as we are above customer expectation we will continue to grow, note that customer expectation will increase over time. performance above the customer expectation will increase cost without any benefit to revenue, while making it easier to stay above the increasing expectation of the customer. 

**QA/QE:** This part has more unit-tests per line of code than any of the levels below and almost as many as Security. 100% of use cases and 95% of corner cases have a unit test.  

**Kano Model: Must-Be Quality**, This is a threshold attribute, unless the product meets the threshold in this area it will soon die due to dissatisfaction. Examples: a Milk carton's ability to not leak. As long as it does not leak, nobody cares about the ability to hold milk. Once it leaks customers become extremely dissatisfied. 

**Quality Tolerance**: Zero   
![][image4]  
Functionality vs Satisfaction: Rarely will higher core functionality improve the customer satisfaction, it needs to be there, it needs to work and that’s it, not working and satisfaction drops very fast. 

# 

# 3 Auxiliary Functionality (Basic Requirement c)  {#3-auxiliary-functionality-(basic-requirement-c)}

![][image5]**Description:** a different type of Basic requirement. This is functionality to support the core functionality, without this it will be very hard for the customer to access the core functionality.  

**Customer perception of need:** for the customer this is so obvious that he need never mention it unprompted unless he had a recent bad experience. He will typically not look for this functionality in a datasheet. This functionality is more visible to the customer than the core functionality, he will see this during a demo or Proof of concept. *The customer will use his perception of the auxiliary functionality to infer the quality of the Core functionality.* 

**On a steam train:** Ability to reverse, dump sand on tracks for steep inclines, a coal tender pulled behind the locomotive. The Coupling that attached the wagons to the locomotive. Ability to sell tickets. 

**Metric:** Measure if and how much feature is used, measure how easy it is for the customer to use, diagnostics metrics 

**QA/QE:** 100% of use cases and 75% of corner cases has a unit test.  

**Kano Model: Must-Be Quality**, This is a threshold attribute, unless the product meets the threshold in this area it will soon die due to dissatisfaction. Examples: a Milk carton's ability to not leak. As long as it does not leak, nobody cares about the ability to hold milk. Once it leaks customers become extremely dissatisfied. 

**Quality Tolerance**: This can be broken for 1-2 days as long as the core functionality keeps working.

![][image4]

**Functionality vs Satisfaction:** Rarely will higher auxiliary functionality improve the customer satisfaction, it needs to be there, it needs to work pretty good, since this is a more visible to the customer, more is required that MVP for customer to be satisfied. 

# 

# 4 Performance functionality  {#4-performance-functionality}

![][image6]**Description:** A Performance metric \- a place where more is better: (not always speed) Unlike Threshold Functionality which are either on or off, Performance functionality exist on a continuum from bad to good where we can always improve. Low performance in this scale will lead to low customer satisfaction and high performance directly corresponds with higher satisfaction. Price closely related to this functionality: higher quality \= higher price are they willing to pay. Performance functionality typically leads to diminishing returns as quality increases, diligence should be used to determine the greatest return on customer satisfaction.  

**Customer perception of need:** This is the main driver for customer purchase and churn decision. Customers will look for this in the datasheet and will compare us with the competition. *Drives objective buying decisions.* 

**On a steam train:** the speed of the train, amount of cargo that can be hauled. 

**On Cars:** Fuel-efficiency

**Metric:**  Measure the performance on this metric, set a goal for acceptable performance. 

**QA/QE: **Performance must be measured under both controlled environments (in the Lab, in staging, Synthetic etc) and as real life customer experiences (in production from end-user perspective) 

**Kano Model: One-dimensional Quality** 

**Quality Tolerance:** Relatively small dips in performance (10%) can be accepted for up to 2 weeks.  
![][image7]

Functionality vs Satisfaction: Linear relationship between performance and satisfaction.

# 

# 5 Bells and Whistles functionality {#5-bells-and-whistles-functionality}

![][image8]**Description:** Gizmos with a Great Wow factor that drives customers to sales. Seen as a great differentiator. Has actual practical value and super slick implementation. Causes a buzz and increases NPS.  
Note: stay away from functionality that is all Wow and no practical use \- This is "Show Horse" functionality see below. 

**Customer perception of need:** Customer will not mention this unprompted, Customer typically didn't realize he had this need until we showed it to them. Once they have seen it they will quickly convince themself that they cannot live without it. Drives emotional buying decisions. 

**On a steam train:** When the locomotive pulls into the station all the kids look at the Bells and Whistles, they are shiny and make noise. Between two similar trains most people will inspect the one with the Bells and Whistles first and most favorably. Bells and Whistles practically serve the purpose of signaling that the train is approaching. 

**Metric:** Measure if and how much a feature is used, diagnostics metrics 

**QA/QE:** 100% of use cases and 50% of corner cases has a unit test.  

**Kano Model: Attractive Quality**, Excitement attributes are for the most part unforeseen by the client but may yield paramount satisfaction. 

**Quality Tolerance**: This can be broken for up to 5 days days as long as the core functionality and auxiliary functionality keeps working. 

**![][image9]**

**Functionality vs Satisfaction:** Even a really poor implementation of a Bells and Whistles function will impress early adopters, exponential excitement as functionality improves. 

# 

# 6 Less is more functionality (and more is worse) {#6-less-is-more-functionality-(and-more-is-worse)}

![][image10]**Description:** Bloatware Gizmo and functionality that when added will actually reduce customer satisfaction. Adds to clutter; introduces extraneous steps to reach core functionality; Introduces distractions; adds the ability for the customer to select the wrong option. **Less is More functionality** **is the deliberate development effort to REMOVE functionality that is in the way of a great outcome.**

**Customer perception of need**: Customers are typically unable to express the need for "less is more" ; they will typically ask for more functionality to solve a problem that is better solved with less functionality. 

**On a steam train:** Ability to smoke cigarettes in the compartments. Ability for passengers to blow the whistle. Japanese style automatic bidet in restrooms with cold water option. The Holman Locomotive with a ridiculously complex set of wheels with no added benefit.

**Metric:** Measure clicks to desired functionality (lower is better). Measure time customers hesitate on a web-page (lower is better). Measure the percentage of time that customers pick the right option (higher is better). 

**In Software:** Automatic adjustments of parameters, good defaults. Fewer options. 

**QA/QE:** Unit tests to ensure that new functionality does not introduce extra steps to reach core functionality. 

**Kano Model: Reverse Quality** 

**Quality Tolerance**: Quarterly of review of UI clutter should be conducted based on metrics.

**![][image11]**

**Functionality vs Satisfaction:** Initial excitement over a new feature quickly turns sour as the new feature gets in the way. expanding on the feature only makes matters worse.

# 7 Me too/checkbox functionality  {#7-me-too/checkbox-functionality}

![][image12]**Description:** For some reason the industry is doing this, customers expect it, but strictly speaking it is neither core nor auxiliary functionality, most of our customers would still be our customers if we didn't have this. Includes features that are Check-box type features in RFC, e.g. customer needs to check the box on the RFC, but will never actually use the feature. Important for new sales, unimportant for churn. Basically the customer saw the feature in a brochure from a competitor and wants it in our product but has no real use for the feature. We make the feature so that we can claim that "we too" has that feature. 

**Customer perception of need:** This is a driver for the customer purchase decision. Customers will look for this in the datasheet and will compare us with the competition. Drives emotional buying decisions. 

**On a steam train:** Heated waiting rooms. 

**Metric:** Measure if and how much feature is used, diagnostics metrics 

**QA/QE:** 100% of use cases and 50% of corner cases has a unit test.  

**Kano Model:** 50/50 Mix between **Attractive Quality** and **Indifferent Quality.** Influences purchasing decisions, no effect on churn decisions.

**![][image13]**

**Functionality vs Satisfaction:** mild unhappiness when function is not there turns to slightly happy once a MVP of functionality is available, since the function will never be used in production improving on it does nothing for the customer. 

# 

# 8 Nice to have functionality {#8-nice-to-have-functionality}

![][image14]**Description:** Items that will make day-to-day life a little easier, but no customer will ever base a buying or churning decision on this functionality. Well-executed "nice to have" functionality will improve NPS but not as much as Bells and Whistles. 

**Customer perception of need:** None. The customer will not mention it unprompted. Customers typically don't miss this functionality until using the product. 

**On a steam train:** time tables sorted alphabetically by destination.  

**In software**: Ability to sort columns in UI 

**Metric:** Measure if and how much feature is used, diagnostics metrics 

**QA/QE:** 100% of use cases and 50% of corner cases has a unit test.  

**Kano Model: Indifferent Quality. **Does not influence customer buying or churn decisions.

![][image15]

**Functionality vs Satisfaction:** Slight annoyance turns to slight happiness as function is implemented and improved, not much variance despite effort.

# 9 Single customer functionality {#9-single-customer-functionality}

**Description**: Functionality that is important to 1 customer only, but hardly relevant to other customers. 

**Customer perception of need:** None. 

**On a steam train:** Ability for the Train stop at Smiths Factory. 

**Metric:** Measure if and how much feature is used, diagnostics metrics. Kill the feature as soon as it is not used any more. 

**QA/QE:** 100% of use cases has a unit test.  

**Kano Model: Indifferent Quality** and **Reverse Quality.** For all except 1 customer does not influence their buying decisions. For the 1 customer this is either paramount (send to deal desk) or Nice to have (don't do it), for everyone else it is Clutter, and distractions, places to choose wrong. 

**![][image11]**

**Functionality vs Satisfaction: **Satisfaction increased for one customer and dissatisfaction increased for all other customers. 

# 10 Show Horse functionality {#10-show-horse-functionality}

![][image16]**Description:** The bad twin to "bells and whistles" and an extreme version of "Less of is more" functionality \- this horse is all show and no work. Gizmos and Gadgets that look great and excite customers but on closer inspection does not deliver any value. A really easy and dangerous trap to fall into, typically designed by people in touch with the zeitgeist but without proper coordination with Subject Matter Experts. Result is a feature that captures the imagination and causes excitement until it is time to deliver at which point the customer experience turns to disbelief and disappointment. 

**Customer perception of need: **Customer will not mention this unprompted, Customer typically didn't realize he had this need until we showed it to him. Once he has seen it he will quickly convince himself that he cannot live without it. Drives emotional buying decisions. Some customers might never notice that this has no real value. Customers with unrewarded expectations will turn nasty as they require the "bugs" be fixed to live up to their unfulfilled expectation, something that can never be done as the feature is inherently flawed and useless. 

**On a steam train:** Steam engine motor cycle \- cool but also completely useless. 

**Metric:** Measure for unused features and Kill them\!

**QA/QE:** Usefulness of new and existing features has to be reviewed by subject matter experts on a regular basis.

**Kano Model:** Starts as **Attractive Quality** and the moves to **Reverse Quality** as feature matures. 

![][image17]

**Functionality vs Satisfaction:** Satisfaction increases in the beginning and then turns into dissatisfaction as the feature does not deliver in spite of continued "improvement".

# Behind the Scenes functionality (Honorable Mention) {#behind-the-scenes-functionality-(honorable-mention)}

![][image18]**Description:** Functionality that improves Company's operations, but means nothing to the internal or external customers, as they won't be aware of it.

Cost reduction features go in this category. 

**Customer perception of need:** None.  

**On a steam train: **Thickness of steel plates, Fuels (woods) optimal burning temperature, time between maintenance. 

**Metric:** Measure as needed 

**QA/QE:** Unit-testing as needed. 

**Kano Model: Indifferent Quality** 

![][image19]

**Functionality vs Satisfaction:** Functionality has no influence on customer satisfaction.

# Functionality changes over time  {#functionality-changes-over-time}

## Cool new Feature life cycle.  {#cool-new-feature-life-cycle.}

Bell and Whistles → Performance → Basic requirement →  Less is more. 

Similar to the Traditional Kano model transition. 

1\. Bell and Whistles: People didn't know this existed but now they want it even if it doesn't do much (Alpha or MVP) 

2\. Performance Functionality: Depending on pressure from competition moves into Performance functionality relatively fast 

3\. Basic Requirement: Stays as a performance metric (sometimes for years) until it becomes a basic requirement and falls off the radar of the customer except for when it is not working. 

4\. Less is more: Function becomes obsolete and starts detracting from the functionality. 

Stream Train analogy 

1\. **Bell and Whistles**: in 1808 people paid money to see an early Locomotive at the "Steam Circus" drive around in circles at a speed of 12 Mph. 

2\. **Performance Functionality**: by 1830 speed was such a factor that Stephenson named his record winning Locomotive "Rocket" as it set a new record of 30 Mph.  

  The Performance era was already over in 1938 when the Mallard set the still unbroken record of 126 Mph for a steam train.

3\. **Basic functionality:** with most Locomotives able to go faster than was safe on the majority of rail tracks other factors such as fuel economy and passenger comfort became important.   
4\. **Less is More**: By 1930 Diesel-Electric Locomotives became the new "Bell's and Whistles" and stream trains were seen as dirty, hard to use and was phased out of production around 1950 

## Competitor's Show Horse Life Cycle.  {#competitor's-show-horse-life-cycle.}

Show Horse → Nice to have → Me too → Less is more. 

1\. Show Horse Functionality. Competitor has a new Whizbang, our investigation shows that the feature has very little use, but customers love it without being able to articulate any practical use. 

2\. Nice to have Functionality. Customers start requesting that we do something similar to Competitor 

3\. Me too Functionality. We end up implementing a minimal version of the competitors feature just to be able to check the box on customers RFP 

4\. Less is more functionality. Eventually the feature falls out of fashion and makes the product look outdated.and we can remove it again.

[image1]: images/figure-01.png
[image2]: images/figure-02.png
[image3]: images/figure-03.png
[image4]: images/figure-04.png
[image5]: images/figure-05.png
[image6]: images/figure-06.png
[image7]: images/figure-07.png
[image8]: images/figure-08.png
[image9]: images/figure-09.png
[image10]: images/figure-10.png
[image11]: images/figure-11.png
[image12]: images/figure-12.png
[image13]: images/figure-13.png
[image14]: images/figure-14.png
[image15]: images/figure-15.png
[image16]: images/figure-16.png
[image17]: images/figure-17.png
[image18]: images/figure-18.png
[image19]: images/figure-19.png