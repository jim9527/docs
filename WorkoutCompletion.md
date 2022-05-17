# WorkoutCompletion Feed Generation logic

## Introduce
A workoutCompletion feed is distinguished by three fields

| type | teamId | source |
| ------ | ------ | ------ |
| FeedType.WorkoutCompletion | coach.teamId | workout._id|

## Use case
1. when coach's teamId not in current player's team
2. Current player completes a workout
3. an empty WorkoutCompletion Feed will be generated in another team(**coach.teamId - coach's current team**)
