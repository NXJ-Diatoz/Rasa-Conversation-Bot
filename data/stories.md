## happy path
* greet
  - utter_greet
* mood_great
  - utter_happy

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot

## interactive_story_1
* greet
    - utter_greet
* tell_issue
    - utter_explain_issue
* explain_issue_Food{"food_name": "noodles", "issue": "spoilt"}
    - slot{"food_name": "noodles"}
    - slot{"issue": "spoilt"}
    - utter_restaurant_query
* restaurant_names{"restaurant_name": "Taj Hotels"}
    - slot{"restaurant_name": "Taj Hotels"}
    - utter_order_number
* Order_number{"order_number": "ORD74IN64CH57"}
    - slot{"order_number": "ORD74IN64CH57"}
    - utter_details_confirm
* affirm
    - utter_happy
    - action_restart
