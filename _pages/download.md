---
layout: default
permalink: "/download"
---

<link rel="stylesheet" type="text/css" href="/static/css/home.css">

<h2 class="anchor" id="download">Download</h2>
<div class="download-container row"  style="margin-top:50px">
  <div class="col-md-6 col-sm-6 col-xs-12 col-12">
    <a class="button-div" href="https://dl.fbaipublicfiles.com/large_objects/MUGEN_release/coinrun.zip">
    Download 3.2s Video Clips Version
    </a>
  </div>

  <div class="col-md-6 col-sm-6 col-xs-12 col-12">
    <a class="button-div" href="https://dl.fbaipublicfiles.com/large_objects/MUGEN_release/full_json_data.zip">
    Download Full Video Version
    </a>
  </div>

  <p>
  NOTE: we have noticed that the download links may not work sometimes. We suspect this is because of network connection issues. If this happens, please try again later.
  </p>
</div>
<hr>

<!-- DATA FORMAT --------------------------------------------------------- -->
<div class="format-container row">
  <div class="col-md-12 col-sm-12 col-xs-12 col-12">
    <h2>Annotations Format</h2>
  </div>
  <div class="col-md-12 col-sm-12 col-xs-12 col-12">
  </div>
  <div class="col-md-12 col-sm-12 col-xs-12 col-12" style= "white-space: nowrap; overflow-x: scroll;">
  The annotation files (within coinrun_dataset_jsons/ folder) are of the following format:
    <pre><code>
    {
        "metadata": {
            'version': 'v2',
            'type': '3.2s',
            'game_events': ['collect_coin', 'kill_monster', 'killed_by_monster', 'collect_gem'],
            'action_verbs': ['jump', 'collect', 'walk', 'run', 'move', 'climb', 'fall', 'turn', 'land', 'drop', 'grab', 'hop', 'kill', 'eat', 'hit', 'die'],
            'characters': ['mugen', 'gem', 'gear', 'bee', 'face', 'slime', 'mouse', 'snail', 'ladybug', 'worm', 'frog', 'barnacle', 'coin'],
            'data_folder': 'dataset/coinrun/coinrun_v2_video_data',
            'split': 'test'
        },
        "data": [
            {
                'video': {
                    'id': 'model_gamev2_fine_tune_squat_penalty_die_reward_1.0_seed_402_level_0469_video_frames_0175_to_0270', 
                    'json_file': 'model_gamev2_fine_tune_squat_penalty_die_reward_1.0_seed_402/video_metadata/model_gamev2_fine_tune_squat_penalty_die_reward_1.0_seed_402_level_0469_video_frames_0175_to_0270.json', 
                    'audio_map_file': 'model_gamev2_fine_tune_squat_penalty_die_reward_1.0_seed_402/audio_semantic_map/audio_map.txt',
                    'world_theme_n': 0, 
                    'audio_file': 'model_gamev2_fine_tune_squat_penalty_die_reward_1.0_seed_402/audios/model_gamev2_fine_tune_squat_penalty_die_reward_1.0_seed_402_level_0469_video_frames_0175_to_0270.wav', 
                    'gt_characters': ['mugen', 'coin', 'gear'], 
                    'game_events': ['collect_coin', 'killed_by_monster'], 
                    'num_frames': 96
                }, 
                'annotations': [
                    {
                        'text': 'Mugen walks to the left, and jumps up to the right to a crate, and jumps down to the right to a platform and collects a coin, and walks to the right, and killed by a gear', 
                        'characters': ['mugen', 'gear', 'coin'], 
                        'actions': ['collect', 'walk', 'jump', 'kill'], 
                        'type': 'auto', # This indicate whether the text is manual or auto annotated.
                    },
                    {
                        'text': 'Mugen moves left then right onto a ladder before dismounting the ladder onto the right of the top platform. It then jumps twice to the right onto a box then onto a coin before walking right into a gear being slain.', 
                        'characters': ['mugen', 'gear', 'coin'], 
                        'actions': ['walk', 'jump', 'move'], 
                        'type': 'manual'
                    }
                    ...
                ]
            }
            ...
        ]
    }
    </code></pre>
  </div>
</div>

<hr>
