# SRS documentation

> A List of User Interfaces
>
> Tags: [`2D Rougelike Game`](../ColorWar/index.md) [`CIS 454`](../CIS454/index.md)
>  
> Author: `Zekai Lin`
>
> Resently Update: `Oct.4 23` `16:18`

## Outline

``` plain text

Outline

Definition

Interface

System Structure



UML diagrams

Requirement


```

## Definitions

| Father |   Word   | Similar Word |             Definition             |    Child     |
| :----: | :------: | :----------: | :--------------------------------: | :----------: |
|        | `player` |  Character   | the 2D object operate by character |              |
|        | `enemy`  |   Mosnter    |    the 2D Object operate by AI     |              |
|        |  `drop`  |              |                                    | `exp`,`coin` |
| `drop` |  `exp`   |              |                                    |              |
| `drop` |  `coin`  |              |                                    |              |
|        |  `gun`   |              |                                    |              |
|        | `bullet` |              |                                    |              |
|        |  `map`   |              |                                    |   `trail`    |
| `map`  | `trail`  |              | Area Player can pick and try guns  |              |
|        |          |              |                                    |              |


||||||

``` plaintext

player 

monster 
    enemy

drops
  exp
  coin

attack
    linary
    mutiliner

wall

```

## Interface List

### General Interfaces List

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

### Interfaces
