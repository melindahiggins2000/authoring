# Exercise Headers

Each exercise has a header consisting of a `title` block and a YAML properties defining the exercise:

{% codetabs name="Video", type="py" -%}
## Video Exercise

```yaml
type: VideoExercise 
lang: r
xp: 50 
video_link: //player.vimeo.com/video/160339466
video_hls: //videos.datacamp.com/transcoded/672_intermediate_r/v2/hls-ch1_1.master.m3u8
```
{%- language name="Normal", type="py" -%}
## Interactive Exercise Title

```yaml
type: NormalExercise
lang: r
xp: 100
```
{%- language name="MultipleChoice", type="py" -%}
## When to use Python?

```yaml
type: MultipleChoiceExercise
lang: python
xp: 50
```
{%- language name="PureMultipleChoice", type="py" -%}
## Example of PureMultipleChoiceExercise

```yaml
type: PureMultipleChoiceExercise
lang: python
xp: 50
```
{%- endcodetabs %}

## Exercise Properties {#exercise-properties}

The supported properties differ depending on the type of the exercise:

| Block          | Video              | Normal             | MultipleChoice     | PureMultipleChoice  |
|----------------|-------------------:|-------------------:|-------------------:|--------------------:|
| `type`         | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| `key`          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| `lang`         | :white_check_mark: | :white_check_mark: | :white_check_mark: | :x:                 |
| `xp`           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:  |
| `video_link`   | :white_check_mark: | :x:                | :x:                | :x:                 |
| `aspect_ratio` | :white_check_mark: | :x:                | :x:                | :x:                 |

- `type`: type of the exercise you are creating as listed in [Exercise Types](README.md#exercise-types).
- `key`: a unique key for the exercise generated by DataCamp. Do not modify or duplicate this key.
- `lang`: the language of the exercise (`r`, `python`, `sql`, or `shell`).
- `xp`: the XP the student will receive for solving the exercise.
- `video_link`: a link to the video for a `VideoExercise`.
- `aspect_ratio`: the aspect ration for a `VideoExercise`.
