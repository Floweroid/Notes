# User Interfaces List

> A List of User Interfaces
>
> Tags: [`ColorWar`](../../view/ColorWar/index.md)
>  
> Author: `Zekai Lin`
>
> Resently Update: `Oct.4 23` `16:18`

## Definitions

| Word | Similar Word | Definition |
|:-:   |   :-:        |   :-:      |
| player |            | the 2D object operate by character |
|Mosnter | enemy |  the 2D Object operate by AI |

``` plaintext

player 

monster 
    enemy

drops
    pigment

attack
    linary
    mutiliner

wall

```

## General Interfaces List

``` yaml
General:

  - mouse

MainMenu: 
  - continue #when there is not completed game
  start new:
    mode choosing:
        demo
  - *config #to configuration
  # todo: history & achievement
  - exit


game:
  inGame:

    - aim

    hint:
        - survival time
    - background
    - character
    - enemies

    attrbuutes:
        - color heading
        - pigment 
        - HP
        - Armor

    - main charater

    bullets: 
        - by enemy
        - by main character
    - mouse 

    stop:
        - restart
        - end
        - *config
        - back to the end 

    use pigment:
        - add attack
        - add hp
        - add armor

    wiki: *wiki

  GameOver:
    - character
    - suvive time
    - kill
    - earn pigment

  wiki: 
    attack:
        - linear
        - coming soon
    enemy:
        - basic
        - coming soon
    drops:
      - pigment

&config configuration:
    - keys
    - sounds
    - color

# todo: playground & color choosing
# todo: collection and color choosing


```


