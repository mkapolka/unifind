# Unifind

Tool for discovering usages of serialized classes within your unity project.
Firstly, you'll need to have your unity files in text serialization mode.
Point it at the .cs file of a MonoBehaviour you wrote and it'll search through your project finding usages of that class.
Currently, it's able to detect:
1. Prefabs using this Monobehaviour
2. Instances of those prefabs in scenes
3. GameObjects within scenes that use that Monobehaviour.

## Usage
```
usage: unifind [-h] [--class-file CLASS_FILE] [--directory PROJECT_ROOT]

Find instances of classes in your unity project

optional arguments:
  -h, --help            show this help message and exit
  --class-file CLASS_FILE, -c CLASS_FILE
                        In which file is the class located?
  --directory PROJECT_ROOT, -d PROJECT_ROOT
                        Where do you want to look for usages?
```
