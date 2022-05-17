# WorkoutCompletion Feed Generation logic

## Introduce
A workoutCompletion feed is distinguished by three fields

| type | teamId | source |
| ------ | ------ | ------ |
| FeedType.WorkoutCompletion | coach.teamId | workout._id|

## Use case
1. When coach's teamId not equal to current player's team id
2. Current player completes a workout
3. An empty WorkoutCompletion Feed will be generated in another team(**coach.teamId - coach's current team**)
