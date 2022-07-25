
# tournament 




## Room List
### Basic Information

**Path：** /open_tournament/room_list

**Method：** GET

**API description：**

### Request Parameters

**Headers**

| Parameters Name | Parameters | If necessary | Examples | Notes |
| ------------ | ------------ | ------------ | ------------ | ------------ |
| Content-Type  |  application/xml | Necessary |   |   |

**Query**

| Parameters Name | If necessary | Examples | Notes |
| ------------ | ------------ | ------------ | ------------ |
|  |  |   |   |

### Return Data

| Name | Type | If necessary | default number | Notes | other information |
| ------------ | ------------ | ------------ |------------ | ------------ | ------------ |
| code | number | necessary |  | 0 ok |   |
| message | string | necessary | | | |
| show_err | boolean | necessary | | | |
| timestamp | number | necessary | | | |
| data | object [] | necessary | | | item type: object |
| #—capacity | number | necessary | | capacity | |
| #—created_at | string | necessary | | created time | |
| #—current_cap | number | necessary | | number of horses currently | |
| #—end_time | number | necessary | | end time of the room is the start time of game | |
| #—id | number | necessary | | room id | |
| #—prize_pool | String | necessary | | prize pool | |
| #—race_id | number | necessary | | Race id | |
| #—start_time | number | necessary | | start time | |
| #—status | number | necessary | | 0. start soon，1. prepare; 2. lock 3. racing 4. finished 5. fail | |
| #—type | number | necessary | | 2: tournament | |
| #—updated_at | String | necessary | | updated time | |


## Room Information
### Basic Information

**Path：** /open_tournament/room

**Method：** GET

**API description：**

### Request Parameters

**Headers**

| Parameters Name | Parameters | If necessary | Examples | Notes |
| ------------ | ------------ | ------------ | ------------ | ------------ |
| Content-Type  |  application/xml | Necessary |   |   |

**Query**

| Parameters Name | If necessary | Examples | Notes |
| ------------ | ------------ | ------------ | ------------ |
| room_id | Necessary | 1 |   |

### Return Data

| Name | Type | If necessary | default number | Notes | other information |
| ------------ | ------------ | ------------ |------------ | ------------ | ------------ |
| code | number | necessary |  | 0 ok |   |
| message | string | necessary | | | |
| show_err | boolean | necessary | | | |
| timestamp | number | necessary | | | |
| data | object | necessary | | | item type: object |
| #—race_id | number | necessary | |  | |
| #—room | object | necessary | |  | |
| #—#—capacity | number | necessary | | capacity | |
| #—#—created_at | string | necessary | | created time | |
| #—#—current_cap | number | necessary | | number of horses currently | |
| #—#—end_time | number | necessary | | end time of the room is the start time of game | |
| #—#—id | number | necessary | | room id | |
| #—#—prize_pool | String | necessary | | prize pool | |
| #—#—race_id | number | necessary | | Race id | |
| #—#—start_time | number | necessary | | start time | |
| #—#—status | number | necessary | | 0. start soon，1. prepare; 2. lock 3. racing 4. finished 5. fail | |
| #—#—type | number | necessary | | 2 tournament | |
| #—#—updated_at | String | necessary | | updated time | |
| #—room_horses | Object[] | necessary | |  | item type: object |
| #—#—acceleration | String | necessary | | acceleration | |
| #—#—aggressiveness | String | necessary | | aggressiveness | |
| #—#—sprint_speed | String | necessary | | sprint_speed | |
| #—#—bloodline | String | necessary | | bloodline | |
| #—#—horse_name | String | necessary | | horse name | |
| #—#—img_url | String | necessary | | horse img | |


## Race Results
### Basic Information

**Path：** /open_tournament/race

**Method：** GET

**API description：**

### Request Parameters

**Headers**

| Parameters Name | Parameters | If necessary | Examples | Notes |
| ------------ | ------------ | ------------ | ------------ | ------------ |
| Content-Type  |  application/xml | Necessary |   |   |

**Query**

| Parameters Name | If necessary | Examples | Notes |
| ------------ | ------------ | ------------ | ------------ |
| race_id | Necessary | 1 |   |

### Return Data

| Name | Type | If necessary | default number | Notes | other information |
| ------------ | ------------ | ------------ |------------ | ------------ | ------------ |
| code | number | necessary |  | 0 ok |   |
| message | string | necessary | | | |
| show_err | boolean | necessary | | | |
| timestamp | number | necessary | | | |
| data | object | necessary | | | item type: object |
| #—shortest_time_elapsed | number | necessary | | shortest time elapsed  | |
| #— start_at | number | necessary | | start time | |
| #—time_elapsed | number | necessary | | longest time elapsed | |
| #—distance | number | necessary | | distance 1200 | |
| #—prize_pool | string | necessary | | prize pool | |
| #—race_id | number | necessary | | race id | |
| #—status | number | necessary | | 1 no start; 2 race run; 3 race end | |
| #—race_name | string | necessary | | race name | |
| #—race_url | string | necessary | | race 3D url| |
| #—racecourse | string | necessary | | racecourse | |
| #—ranking | object[] | necessary | |  | item type: object |
| #—#—award | string | necessary | | gain rewards | |
| #—#—color | object | necessary | | color | |
| #—#—#—B | number | necessary | |  | |
| #—#—#—G | number | necessary | |  | |
| #—#—#—R | number | necessary | |  | |
| #—#—acceleration | String | necessary | | acceleration | |
| #—#—aggressiveness | String | necessary | | aggressiveness | |
| #—#—sprint_speed | String | necessary | | sprint_speed | |
| #—#—bloodline | String | necessary | | bloodline | |
| #—#—horse_id | number | necessary | |  | |
| #—#—user_id | number | necessary | |  | |
| #—#—wallet_addr | number | necessary | |  | |
| #—#—horse_name | String | necessary | | horse name | |
| #—#—img_url | String | necessary | | horse img | |
| #—#—gate | number | necessary | | gate | |
| #—#—rank | number | necessary | | rank | |
| #—#—time_elapsed | number | necessary | | time elapsed | |
