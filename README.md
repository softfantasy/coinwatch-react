# Coinwatch

- real-time cryptocurrency ticker, order, contracts

## Table of Contents

1. [About](#about)
2. [Development Environment](#development-environment)
3. [Getting Started](#getting-started)
4. [Folder Structure](#folder-structure)
5. [Screenshots](#screenshots)
   - [coin_home](#coin_home)
   - [coin_show](#coin_show)
6. [Todo](#todo)

## About


## Development Environment

- React(v16.3.1) + Redux(v3.7.2)
- node.js(v8.10.0), html, css, Bootstrap4
- [cyptocompare api](https://www.cryptocompare.com/api/)
- [bithumb api](https://www.bithumb.com/u1/US127)

## Getting Started

```
$ npm install
$ npm start
```

**Note** -   If loading animation continues when you start this project, install this chrome extensions : https://chrome.google.com/webstore/detail/allow-control-allow-origi/nlfbmbojpeacfghkpbjhddihlkkiljbi?utm_source=chrome-ntp-icon

and turn on *Enable cross-origin resource sharing* in the settings of this program. 

## Folder Structure

```
Coinwatch_web/
  ~
  src/
    actions/
      index.js
    components/
      chart_in_coin_home.js
      chart_in_coin_show.js
      coin_card.js
      coin_info_tabs.js
      coin_info_top.js
      coin_list.js
      contracts.js
      header_home.js
      header_show.js
      order_book.js
    containers/
      coin_home.js
      coin_show.js
    img/
      sky.jpg
    reducers/
      coin_list_reducer.js
      coin_reducer.js
      index.js
    App.css
    App.js
    index.css
    index.js
```



## Screenshots

#### *coin_home*

![coin_home_screen](https://screenshot-for-github.s3.ap-northeast-2.amazonaws.com/GIF3.gif)

```
┌--------------------------coin_home.js--------------------------┐
| ┌-----------------------header_home.js-----------------------┐ |
| |                                                            | |
| └------------------------------------------------------------┘ |
| ┌------------------------coin_list.js------------------------┐ |
| | ┌coin_card.js┐                                             | |
| | |            |                                             | |
| | └------------┘                                             | |
| |                                                            | |
| |                                                            | |
| |                                                            | |
| |                                                            | |
| └------------------------------------------------------------┘ |
└----------------------------------------------------------------┘
```

<br>

#### *coin_show*

![coin_show_screen](https://screenshot-for-github.s3.ap-northeast-2.amazonaws.com/desc3.gif)

```
┌--------------------------coin_show.js--------------------------┐
| ┌-----------------------header_show.js-----------------------┐ |                              
| └------------------------------------------------------------┘ |
| ┌-----------coin_info_top.js------------┐  ┌--order_book.js--┐ |
| |                                       |  |                 | |
| └---------------------------------------┘  |                 | |
| ┌--------chart_in_coin_show.js----------┐  |                 | |		  	
| |                                       |  └-----------------┘ |		
| |                                       |  ┌--contracts.js--┐  |
| |                                       |  |                |  |
| └---------------------------------------┘  |                |  |
| ┌----------coin_info_tabs.js------------┐  |                |  |
| |                                       |  |                |  |
| └---------------------------------------┘  └----------------┘  |
└----------------------------------------------------------------┘
```

<br>
