# A dataset for the in-situ contexts where users perceive smartphone distractions

We collected in-situ user context and the corresponding smartphone distraction experiences. For this, we implemented an mobile esm app that asks users to report their current contexts (i.e., their locations and activities) and to what extent they smartphone distraction. We performed a field data collection study with 34 participants using the app. During three weeks of the data collection session, we collected 9,180 ESM responses from 34 participants. We received an average of 270.0 (SD = 89.8) responses per participant. The results of analysis on this dataset was published in the proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies (IMWUT) [1]

## Detecting moments for response sampling

Requesting responses from users at inappropriate times can cause inconvenience for users, as it may interfere with their ongoing activities. Therefore, finding the right opportunity for sampling experience is essential [2]. Our approach was capturing a time slot during which one activity lasts and asking users to report the context during that time slot rather than asking whenever users turn on their smartphones. We also assumed that when continuing the activity, a user would be stationary, since when the user moves, their context may change. We also only considered the time slot during which users did not use smartphones because their smartphone use may not be related to the activity they are currently engaged in and most importantly, our goal was to identify in what contexts users perceive smartphones as distracting. Therefore, to determine when to display the survey screen in the lockscreen, we decided that two conditions should be satisfied: (1) the user is stationary and (2) the user has not been using their smartphone for a certain amount of time. The app has an internal timer to count to three minutes. If either condition is not satisfied, the app will reset the timer. Once both conditions have continued to be met for three minutes, the app will display the survey lock screen when the user turns on their smartphone. We empirically selected three minutes as the minimum duration of time slot. Once the app detects an opportunity for context sampling, it asked the users to report their current contexts during the captured time slot and the perception of distractions caused by smartphones (See the figure below).

![alt text](https://github.com/Kaist-ICLab/positive-computing-distracting-context/blob/1bc5f9937d0e1f9be6b0febb0531829f439b35b5/esm_app_screen.jpg?raw=true)

## Dataset

Dataset file (dataset.csv) has 10 fields, described as below
1. pid: The ID for each participant of the study
2. location: 
3. activity:
4. start_time:
5. end_time:
6. duration_sec:
7. actual_concentration:
8. expected_concentration:
9. perceived_distraction:
10. purpose_of_using_smartphone: 

## Reference
[1] Kim, Inyeop, et al. "Understanding User Contexts and Coping Strategies for Context-Aware Phone Distraction Management System Design." Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies 4.4 (2020): 1-33.
[2] Choi, Woohyeok, et al. "Multi-stage receptivity model for mobile just-in-time health intervention." Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies 3.2 (2019): 1-26.
