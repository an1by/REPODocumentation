# List of default enemies

For [RepoLib](https://thunderstore.io/c/repo/p/Zehs/REPOLib/)

## Signle enemies
* Ceiling Eye
* Thin Man
* Gnome
* Duck
* Slow Mouth
* Valuable Thrower
* Animal
* Upscream
* Hidden
* Tumbler
* Bowtie
* Floater
* Bang
* Head
* Robe
* Hunter
* Runner
* Beamer
* Slow Walker
> In-code format: `Enemy - <name>`

## Enemy groups
* 3 Animals
* 3 Bowties
* 3 Floaters
* 2 Hidden
* 3 Tumblers
* 3 Upscreams
* 3 Valuable Throwers
* 4 Ceiling Eyes
* 4 Ducks
* 4 Slow Mouths
* 4 Thin Men
* 6 Bangs
* 10 Gnomes
> In-code format: `Enemy Group - <name>`

## How it found
```c#
var instance = EnemyDirector.instance;

List<EnemySetup> lists = new();
lists.AddRange(instance.enemiesDifficulty1);
lists.AddRange(instance.enemiesDifficulty2);
lists.AddRange(instance.enemiesDifficulty3);

foreach (var registeredEnemy in lists)
{
    Console.WriteLine(registeredEnemy.name);
}
```
