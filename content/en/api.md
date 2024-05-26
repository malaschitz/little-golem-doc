---
title: "API"
date: 2023-04-16
weight: 900
description: >
  API for Litle Golem
---

The REST api is used. Examples are given for the curl program. 

# Login

```
curl  -X POST https://api.littlegolem.net/admin/loginPassword 
-d '{"email":"myemail@gmail.com", "password":"aabbccdd"}'
```

```
{
  "version": "1.0",
  "valid": true,
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MTQyMDg3LCJ0aW1lIjoiU3VuIEFwciAxNiAxNDozODowNSAyMDIzIn0.gIrYE-Hckxad_gt5XT-AI5ji3M8bSKjuv4_l_npABCD",
  "on_move": 5,
  "player": {
    "plid": 142087,
    "real_name": "tester111",
    "membership": false,
    "country": "US"
  },
  "players": 59504,
  "games": 2364415,
  "email": "myemail@gmail.com",
  "ulid": "",
  "vacation": 0,
  "mobile_key": "lg1664698498381vihiabcde"
}
```

# Tournament info

```
curl -H "Authorization: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MTQyMDg3LCJ0aW1lIjoiU3VuIEFwciAxNiAxNDozODowNSAyMDIzIn0.gIrYE-Hckxad_gt5XT-AI5ji3M8bSKjuv4_l_npABCD"
-X GET https://api.littlegolem.net/trn/trndetail/go19.cv.GO9.53.2.1
```

```
{
  "trnid": "go19.cv.GO9.53.2.1",
  "gtype": "go19",
  "variant": "GO9",
  "trntyp": "cv",
  "startdate": 1648452685078,
  "finishdate": 1652844655969,
  "players": [
    {
      "player": {
        "player": {
          "plid": 144760,
          "real_name": "galispiar",
          "membership": false,
          "country": "JP"
        },
        "rating": 1021.5246,
        "deviation": 20
      },
      "points": "0",
      "sb": "0",
      "games": "8"
    },
    {
      "player": {
        "player": {
          "plid": 1017,
          "real_name": "Elisa Kabiljo",
          "membership": false,
          "country": "RS"
        },
        "rating": 1698.1548,
        "deviation": 20
      },
      "points": "4",
      "sb": "8",
      "games": "8"
    },
    {
      "player": {
        "player": {
          "plid": 21042,
          "real_name": "drToma",
          "membership": false,
          "country": "RO"
        },
        "rating": 1707.7354,
        "deviation": 20
      },
      "points": "4",
      "sb": "12",
      "games": "8"
    },
    {
      "player": {
        "player": {
          "plid": 4090,
          "real_name": "David Milne",
          "membership": true,
          "country": "NZ"
        },
        "rating": 1551.7124,
        "deviation": 20
      },
      "points": "6",
      "sb": "24",
      "games": "8"
    },
    {
      "player": {
        "player": {
          "plid": 22709,
          "real_name": "Thierry Pertuy",
          "membership": false,
          "country": "FR"
        },
        "rating": 1756.0692,
        "deviation": 20
      },
      "points": "8",
      "sb": "28",
      "games": "8"
    },
    {
      "player": {
        "player": {
          "plid": 44616,
          "real_name": "nullptr",
          "membership": false,
          "country": "US"
        },
        "rating": 1737.2621,
        "deviation": 20
      },
      "points": "8",
      "sb": "32",
      "games": "8"
    },
    {
      "player": {
        "player": {
          "plid": 8262,
          "real_name": "Zandor",
          "membership": false,
          "country": "AT"
        },
        "rating": 1716.0134,
        "deviation": 20
      },
      "points": "12",
      "sb": "60",
      "games": "8"
    },
    {
      "player": {
        "player": {
          "plid": 152553,
          "real_name": "pacmaniac",
          "membership": false,
          "country": "EU"
        },
        "rating": 1825.2876,
        "deviation": 31
      },
      "points": "14",
      "sb": "84",
      "games": "8"
    },
    {
      "player": {
        "player": {
          "plid": 4152,
          "real_name": "Liviu",
          "membership": false,
          "country": "RO"
        },
        "rating": 1910.1044,
        "deviation": 20
      },
      "points": "16",
      "sb": "112",
      "games": "8"
    }
  ],
  "games": [
    {
      "gid": 2302353,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 21042,
            "real_name": "drToma",
            "membership": false,
            "country": "RO"
          },
          "rating": 1707.7354,
          "deviation": 20
        },
        {
          "player": {
            "plid": 4152,
            "real_name": "Liviu",
            "membership": false,
            "country": "RO"
          },
          "rating": 1910.1044,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 0,
      "expire_time": 1650826487655,
      "chngr": [
        -5.220499,
        5.220499
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685080,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 21042,
          "movetime": 1648467119735,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 2,
          "plid": 4152,
          "movetime": 1648489048532,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 3,
          "plid": 21042,
          "movetime": 1648490701910,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 4,
          "plid": 4152,
          "movetime": 1648491302186,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 5,
          "plid": 21042,
          "movetime": 1648563295955,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 6,
          "plid": 4152,
          "movetime": 1648573692727,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 7,
          "plid": 21042,
          "movetime": 1648734770400,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 8,
          "plid": 4152,
          "movetime": 1648748362049,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 9,
          "plid": 21042,
          "movetime": 1649097485668,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 10,
          "plid": 4152,
          "movetime": 1649097592696,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 11,
          "plid": 21042,
          "movetime": 1649169801707,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 12,
          "plid": 4152,
          "movetime": 1649177644159,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 13,
          "plid": 21042,
          "movetime": 1649326134417,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 14,
          "plid": 4152,
          "movetime": 1649351323825,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 15,
          "plid": 21042,
          "movetime": 1649352330875,
          "jmove": "af",
          "dmove": "A6"
        },
        {
          "nmove": 16,
          "plid": 4152,
          "movetime": 1649358621024,
          "jmove": "bc",
          "dmove": "B3"
        },
        {
          "nmove": 17,
          "plid": 21042,
          "movetime": 1649425542645,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 18,
          "plid": 4152,
          "movetime": 1649442037047,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 19,
          "plid": 21042,
          "movetime": 1649593863223,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 20,
          "plid": 4152,
          "movetime": 1649612613634,
          "jmove": "bb",
          "dmove": "B2"
        },
        {
          "nmove": 21,
          "plid": 21042,
          "movetime": 1649616957060,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 22,
          "plid": 4152,
          "movetime": 1649619699326,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 23,
          "plid": 21042,
          "movetime": 1649670751588,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 24,
          "plid": 4152,
          "movetime": 1649691459381,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 25,
          "plid": 21042,
          "movetime": 1649694585297,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 26,
          "plid": 4152,
          "movetime": 1649695829676,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 27,
          "plid": 21042,
          "movetime": 1649696736606,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 28,
          "plid": 4152,
          "movetime": 1649699301733,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 29,
          "plid": 21042,
          "movetime": 1649773761522,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 30,
          "plid": 4152,
          "movetime": 1649779690792,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 31,
          "plid": 21042,
          "movetime": 1649859923395,
          "jmove": "bh",
          "dmove": "B8"
        },
        {
          "nmove": 32,
          "plid": 4152,
          "movetime": 1649864786929,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 33,
          "plid": 21042,
          "movetime": 1649871470074,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 34,
          "plid": 4152,
          "movetime": 1649872943996,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 35,
          "plid": 21042,
          "movetime": 1649873480056,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 36,
          "plid": 4152,
          "movetime": 1649873738401,
          "jmove": "bi",
          "dmove": "B9"
        },
        {
          "nmove": 37,
          "plid": 21042,
          "movetime": 1649874779454,
          "jmove": "ah",
          "dmove": "A8"
        },
        {
          "nmove": 38,
          "plid": 4152,
          "movetime": 1649875711488,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 39,
          "plid": 21042,
          "movetime": 1649953562102,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 40,
          "plid": 4152,
          "movetime": 1649953629828,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 41,
          "plid": 21042,
          "movetime": 1649953837929,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 42,
          "plid": 4152,
          "movetime": 1649953917257,
          "jmove": "ae",
          "dmove": "A5"
        },
        {
          "nmove": 43,
          "plid": 21042,
          "movetime": 1649959806891,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 44,
          "plid": 4152,
          "movetime": 1649960201706,
          "jmove": "ai",
          "dmove": "A9"
        },
        {
          "nmove": 45,
          "plid": 21042,
          "movetime": 1649961306268,
          "jmove": "fa",
          "dmove": "F1"
        },
        {
          "nmove": 46,
          "plid": 4152,
          "movetime": 1649966404954,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 47,
          "plid": 21042,
          "movetime": 1650238106152,
          "jmove": "ea",
          "dmove": "E1"
        },
        {
          "nmove": 48,
          "plid": 4152,
          "movetime": 1650255361103,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 49,
          "plid": 21042,
          "movetime": 1650385455811,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 50,
          "plid": 4152,
          "movetime": 1650392665449,
          "jmove": "ag",
          "dmove": "A7"
        },
        {
          "nmove": 51,
          "plid": 21042,
          "movetime": 1650463422211,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 52,
          "plid": 4152,
          "movetime": 1650470410004,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 53,
          "plid": 21042,
          "movetime": 1650711194924,
          "jmove": "ga",
          "dmove": "G1"
        },
        {
          "nmove": 54,
          "plid": 4152,
          "movetime": 1650716562521,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 55,
          "plid": 21042,
          "movetime": 1650797940123,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 56,
          "plid": 4152,
          "movetime": 1650798164520,
          "jmove": "scorefe",
          "dmove": "Score"
        },
        {
          "nmove": 57,
          "plid": 21042,
          "movetime": 1650826487650,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        727200000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302354,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 4152,
            "real_name": "Liviu",
            "membership": false,
            "country": "RO"
          },
          "rating": 1910.1044,
          "deviation": 20
        },
        {
          "player": {
            "plid": 22709,
            "real_name": "Thierry Pertuy",
            "membership": false,
            "country": "FR"
          },
          "rating": 1756.0692,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 22709,
      "expire_time": 1649227580149,
      "chngr": [
        5.2260504,
        -5.2260504
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685086,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 4152,
          "movetime": 1648489029346,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 2,
          "plid": 22709,
          "movetime": 1648500305231,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 3,
          "plid": 4152,
          "movetime": 1648528199018,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 4,
          "plid": 22709,
          "movetime": 1648539840883,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 5,
          "plid": 4152,
          "movetime": 1648549195301,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 6,
          "plid": 22709,
          "movetime": 1648571415196,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 7,
          "plid": 4152,
          "movetime": 1648573696543,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 8,
          "plid": 22709,
          "movetime": 1648594958828,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 9,
          "plid": 4152,
          "movetime": 1648615675214,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 10,
          "plid": 22709,
          "movetime": 1648629458186,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 11,
          "plid": 4152,
          "movetime": 1648645931561,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 12,
          "plid": 22709,
          "movetime": 1648649810378,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 13,
          "plid": 4152,
          "movetime": 1648656123096,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 14,
          "plid": 22709,
          "movetime": 1648662991918,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 15,
          "plid": 4152,
          "movetime": 1648663934941,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 16,
          "plid": 22709,
          "movetime": 1648669976118,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 17,
          "plid": 4152,
          "movetime": 1648670377429,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 18,
          "plid": 22709,
          "movetime": 1648744250424,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 19,
          "plid": 4152,
          "movetime": 1648748377753,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 20,
          "plid": 22709,
          "movetime": 1648750345332,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 21,
          "plid": 4152,
          "movetime": 1648755603473,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 22,
          "plid": 22709,
          "movetime": 1648757076503,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 23,
          "plid": 4152,
          "movetime": 1648758087906,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 24,
          "plid": 22709,
          "movetime": 1648761668330,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 25,
          "plid": 4152,
          "movetime": 1648769132778,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 26,
          "plid": 22709,
          "movetime": 1648938546079,
          "jmove": "ea",
          "dmove": "E1"
        },
        {
          "nmove": 27,
          "plid": 4152,
          "movetime": 1648985273501,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 28,
          "plid": 22709,
          "movetime": 1649010124347,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 29,
          "plid": 4152,
          "movetime": 1649012281625,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 30,
          "plid": 22709,
          "movetime": 1649017869496,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 31,
          "plid": 4152,
          "movetime": 1649028941679,
          "jmove": "bb",
          "dmove": "B2"
        },
        {
          "nmove": 32,
          "plid": 22709,
          "movetime": 1649053936526,
          "jmove": "ba",
          "dmove": "B1"
        },
        {
          "nmove": 33,
          "plid": 4152,
          "movetime": 1649081441615,
          "jmove": "bc",
          "dmove": "B3"
        },
        {
          "nmove": 34,
          "plid": 22709,
          "movetime": 1649081853410,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 35,
          "plid": 4152,
          "movetime": 1649081910299,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 36,
          "plid": 22709,
          "movetime": 1649082130476,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 37,
          "plid": 4152,
          "movetime": 1649083094103,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 38,
          "plid": 22709,
          "movetime": 1649091043117,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 39,
          "plid": 4152,
          "movetime": 1649092078345,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 40,
          "plid": 22709,
          "movetime": 1649106330661,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 41,
          "plid": 4152,
          "movetime": 1649132558587,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 42,
          "plid": 22709,
          "movetime": 1649139052814,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 43,
          "plid": 4152,
          "movetime": 1649162538470,
          "jmove": "bh",
          "dmove": "B8"
        },
        {
          "nmove": 44,
          "plid": 22709,
          "movetime": 1649173530354,
          "jmove": "ah",
          "dmove": "A8"
        },
        {
          "nmove": 45,
          "plid": 4152,
          "movetime": 1649177659884,
          "jmove": "af",
          "dmove": "A6"
        },
        {
          "nmove": 46,
          "plid": 22709,
          "movetime": 1649188915367,
          "jmove": "ag",
          "dmove": "A7"
        },
        {
          "nmove": 47,
          "plid": 4152,
          "movetime": 1649191014534,
          "jmove": "ab",
          "dmove": "A2"
        },
        {
          "nmove": 48,
          "plid": 22709,
          "movetime": 1649195274198,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 49,
          "plid": 4152,
          "movetime": 1649221693604,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 50,
          "plid": 22709,
          "movetime": 1649227580139,
          "jmove": "resign",
          "dmove": "resign"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302355,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 1017,
            "real_name": "Elisa Kabiljo",
            "membership": false,
            "country": "RS"
          },
          "rating": 1698.1548,
          "deviation": 20
        },
        {
          "player": {
            "plid": 4152,
            "real_name": "Liviu",
            "membership": false,
            "country": "RO"
          },
          "rating": 1910.1044,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 1017,
      "expire_time": 1649829063365,
      "chngr": [
        -4.296472,
        4.296472
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685090,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 1017,
          "movetime": 1648457751957,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 2,
          "plid": 4152,
          "movetime": 1648489040381,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 3,
          "plid": 1017,
          "movetime": 1648506645176,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 4,
          "plid": 4152,
          "movetime": 1648528202268,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 5,
          "plid": 1017,
          "movetime": 1648534639567,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 6,
          "plid": 4152,
          "movetime": 1648549192302,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 7,
          "plid": 1017,
          "movetime": 1648576038798,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 8,
          "plid": 4152,
          "movetime": 1648579560302,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 9,
          "plid": 1017,
          "movetime": 1648584688999,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 10,
          "plid": 4152,
          "movetime": 1648584846339,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 11,
          "plid": 1017,
          "movetime": 1648585392534,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 12,
          "plid": 4152,
          "movetime": 1648586458761,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 13,
          "plid": 1017,
          "movetime": 1648618882378,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 14,
          "plid": 4152,
          "movetime": 1648645919731,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 15,
          "plid": 1017,
          "movetime": 1648659215134,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 16,
          "plid": 4152,
          "movetime": 1648659591575,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 17,
          "plid": 1017,
          "movetime": 1648679583737,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 18,
          "plid": 4152,
          "movetime": 1648701656641,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 19,
          "plid": 1017,
          "movetime": 1648717307035,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 20,
          "plid": 4152,
          "movetime": 1648724688652,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 21,
          "plid": 1017,
          "movetime": 1649532372673,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 22,
          "plid": 4152,
          "movetime": 1649533510233,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 23,
          "plid": 1017,
          "movetime": 1649567712096,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 24,
          "plid": 4152,
          "movetime": 1649572774584,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 25,
          "plid": 1017,
          "movetime": 1649609849576,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 26,
          "plid": 4152,
          "movetime": 1649612635122,
          "jmove": "hi",
          "dmove": "H9"
        },
        {
          "nmove": 27,
          "plid": 1017,
          "movetime": 1649614076859,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 28,
          "plid": 4152,
          "movetime": 1649616930830,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 29,
          "plid": 1017,
          "movetime": 1649829063359,
          "jmove": "resign",
          "dmove": "resign"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        507600000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302356,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 4152,
            "real_name": "Liviu",
            "membership": false,
            "country": "RO"
          },
          "rating": 1910.1044,
          "deviation": 20
        },
        {
          "player": {
            "plid": 8262,
            "real_name": "Zandor",
            "membership": false,
            "country": "AT"
          },
          "rating": 1716.0134,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 0,
      "expire_time": 1651107263442,
      "chngr": [
        4.3720512,
        -4.3720512
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685092,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 4152,
          "movetime": 1648489032018,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 2,
          "plid": 8262,
          "movetime": 1648511119292,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 3,
          "plid": 4152,
          "movetime": 1648528206292,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 4,
          "plid": 8262,
          "movetime": 1648559320624,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 5,
          "plid": 4152,
          "movetime": 1648559370027,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 6,
          "plid": 8262,
          "movetime": 1648559377729,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 7,
          "plid": 4152,
          "movetime": 1648573680661,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 8,
          "plid": 8262,
          "movetime": 1648665915270,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 9,
          "plid": 4152,
          "movetime": 1648668660604,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 10,
          "plid": 8262,
          "movetime": 1648838615953,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 11,
          "plid": 4152,
          "movetime": 1648855340970,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 12,
          "plid": 8262,
          "movetime": 1648922678588,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 13,
          "plid": 4152,
          "movetime": 1648985259277,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 14,
          "plid": 8262,
          "movetime": 1649096050510,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 15,
          "plid": 4152,
          "movetime": 1649097586698,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 16,
          "plid": 8262,
          "movetime": 1649108185259,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 17,
          "plid": 4152,
          "movetime": 1649132577550,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 18,
          "plid": 8262,
          "movetime": 1649166375957,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 19,
          "plid": 4152,
          "movetime": 1649177640691,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 20,
          "plid": 8262,
          "movetime": 1649346316294,
          "jmove": "bh",
          "dmove": "B8"
        },
        {
          "nmove": 21,
          "plid": 4152,
          "movetime": 1649351334216,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 22,
          "plid": 8262,
          "movetime": 1649443851747,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 23,
          "plid": 4152,
          "movetime": 1649444912986,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 24,
          "plid": 8262,
          "movetime": 1649525815460,
          "jmove": "bi",
          "dmove": "B9"
        },
        {
          "nmove": 25,
          "plid": 4152,
          "movetime": 1649528245170,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 26,
          "plid": 8262,
          "movetime": 1649631123515,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 27,
          "plid": 4152,
          "movetime": 1649651436964,
          "jmove": "ae",
          "dmove": "A5"
        },
        {
          "nmove": 28,
          "plid": 8262,
          "movetime": 1649688245210,
          "jmove": "af",
          "dmove": "A6"
        },
        {
          "nmove": 29,
          "plid": 4152,
          "movetime": 1649691468198,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 30,
          "plid": 8262,
          "movetime": 1649709222662,
          "jmove": "ag",
          "dmove": "A7"
        },
        {
          "nmove": 31,
          "plid": 4152,
          "movetime": 1649738659441,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 32,
          "plid": 8262,
          "movetime": 1649862284794,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 33,
          "plid": 4152,
          "movetime": 1649864807844,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 34,
          "plid": 8262,
          "movetime": 1649865067983,
          "jmove": "ih",
          "dmove": "I8"
        },
        {
          "nmove": 35,
          "plid": 4152,
          "movetime": 1649865193594,
          "jmove": "ha",
          "dmove": "H1"
        },
        {
          "nmove": 36,
          "plid": 8262,
          "movetime": 1649937465637,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 37,
          "plid": 4152,
          "movetime": 1649937629596,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 38,
          "plid": 8262,
          "movetime": 1649937648432,
          "jmove": "hi",
          "dmove": "H9"
        },
        {
          "nmove": 39,
          "plid": 4152,
          "movetime": 1649950912098,
          "jmove": "fi",
          "dmove": "F9"
        },
        {
          "nmove": 40,
          "plid": 8262,
          "movetime": 1649956354312,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 41,
          "plid": 4152,
          "movetime": 1649956428808,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 42,
          "plid": 8262,
          "movetime": 1649966351517,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 43,
          "plid": 4152,
          "movetime": 1649966408612,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 44,
          "plid": 8262,
          "movetime": 1649967259540,
          "jmove": "gi",
          "dmove": "G9"
        },
        {
          "nmove": 45,
          "plid": 4152,
          "movetime": 1649967662361,
          "jmove": "ib",
          "dmove": "I2"
        },
        {
          "nmove": 46,
          "plid": 8262,
          "movetime": 1650230608375,
          "jmove": "ic",
          "dmove": "I3"
        },
        {
          "nmove": 47,
          "plid": 4152,
          "movetime": 1650255357904,
          "jmove": "ga",
          "dmove": "G1"
        },
        {
          "nmove": 48,
          "plid": 8262,
          "movetime": 1650367247011,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 49,
          "plid": 4152,
          "movetime": 1650372715849,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 50,
          "plid": 8262,
          "movetime": 1650587652058,
          "jmove": "ia",
          "dmove": "I1"
        },
        {
          "nmove": 51,
          "plid": 4152,
          "movetime": 1650606140796,
          "jmove": "id",
          "dmove": "I4"
        },
        {
          "nmove": 52,
          "plid": 8262,
          "movetime": 1650805351920,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 53,
          "plid": 4152,
          "movetime": 1650806628015,
          "jmove": "ib",
          "dmove": "I2"
        },
        {
          "nmove": 54,
          "plid": 8262,
          "movetime": 1650812114470,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 55,
          "plid": 4152,
          "movetime": 1650814535156,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 56,
          "plid": 8262,
          "movetime": 1650826098277,
          "jmove": "ia",
          "dmove": "I1"
        },
        {
          "nmove": 57,
          "plid": 4152,
          "movetime": 1650826901910,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 58,
          "plid": 8262,
          "movetime": 1650891546877,
          "jmove": "ib",
          "dmove": "I2"
        },
        {
          "nmove": 59,
          "plid": 4152,
          "movetime": 1650892414587,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 60,
          "plid": 8262,
          "movetime": 1651015127577,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 61,
          "plid": 4152,
          "movetime": 1651033736536,
          "jmove": "scoreidfc",
          "dmove": "Score"
        },
        {
          "nmove": 62,
          "plid": 8262,
          "movetime": 1651107263435,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302357,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 44616,
            "real_name": "nullptr",
            "membership": false,
            "country": "US"
          },
          "rating": 1737.2621,
          "deviation": 20
        },
        {
          "player": {
            "plid": 4152,
            "real_name": "Liviu",
            "membership": false,
            "country": "RO"
          },
          "rating": 1910.1044,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 0,
      "expire_time": 1649572737970,
      "chngr": [
        -4.1699247,
        4.1699247
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685094,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 44616,
          "movetime": 1648516030760,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 2,
          "plid": 4152,
          "movetime": 1648528213875,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 3,
          "plid": 44616,
          "movetime": 1648603497043,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 4,
          "plid": 4152,
          "movetime": 1648615689689,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 5,
          "plid": 44616,
          "movetime": 1648628180953,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 6,
          "plid": 4152,
          "movetime": 1648645928086,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 7,
          "plid": 44616,
          "movetime": 1648690345342,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 8,
          "plid": 4152,
          "movetime": 1648701663019,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 9,
          "plid": 44616,
          "movetime": 1648729868213,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 10,
          "plid": 4152,
          "movetime": 1648748351813,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 11,
          "plid": 44616,
          "movetime": 1648775797431,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 12,
          "plid": 4152,
          "movetime": 1648788512459,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 13,
          "plid": 44616,
          "movetime": 1648856743626,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 14,
          "plid": 4152,
          "movetime": 1648876169781,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 15,
          "plid": 44616,
          "movetime": 1648951833013,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 16,
          "plid": 4152,
          "movetime": 1648985276986,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 17,
          "plid": 44616,
          "movetime": 1648997048825,
          "jmove": "bc",
          "dmove": "B3"
        },
        {
          "nmove": 18,
          "plid": 4152,
          "movetime": 1648998257209,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 19,
          "plid": 44616,
          "movetime": 1649012088891,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 20,
          "plid": 4152,
          "movetime": 1649012314620,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 21,
          "plid": 44616,
          "movetime": 1649019715365,
          "jmove": "ig",
          "dmove": "I7"
        },
        {
          "nmove": 22,
          "plid": 4152,
          "movetime": 1649028957633,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 23,
          "plid": 44616,
          "movetime": 1649037571130,
          "jmove": "ie",
          "dmove": "I5"
        },
        {
          "nmove": 24,
          "plid": 4152,
          "movetime": 1649047274096,
          "jmove": "ih",
          "dmove": "I8"
        },
        {
          "nmove": 25,
          "plid": 44616,
          "movetime": 1649077004700,
          "jmove": "if",
          "dmove": "I6"
        },
        {
          "nmove": 26,
          "plid": 4152,
          "movetime": 1649081481658,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 27,
          "plid": 44616,
          "movetime": 1649129235130,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 28,
          "plid": 4152,
          "movetime": 1649132645098,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 29,
          "plid": 44616,
          "movetime": 1649206927257,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 30,
          "plid": 4152,
          "movetime": 1649221731303,
          "jmove": "af",
          "dmove": "A6"
        },
        {
          "nmove": 31,
          "plid": 44616,
          "movetime": 1649294056772,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 32,
          "plid": 4152,
          "movetime": 1649305811573,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 33,
          "plid": 44616,
          "movetime": 1649359874071,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 34,
          "plid": 4152,
          "movetime": 1649360949469,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 35,
          "plid": 44616,
          "movetime": 1649375275610,
          "jmove": "ac",
          "dmove": "A3"
        },
        {
          "nmove": 36,
          "plid": 4152,
          "movetime": 1649390088123,
          "jmove": "ae",
          "dmove": "A5"
        },
        {
          "nmove": 37,
          "plid": 44616,
          "movetime": 1649429854246,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 38,
          "plid": 4152,
          "movetime": 1649442045631,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 39,
          "plid": 44616,
          "movetime": 1649562659907,
          "jmove": "score",
          "dmove": "Score"
        },
        {
          "nmove": 40,
          "plid": 4152,
          "movetime": 1649572737965,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302358,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 4152,
            "real_name": "Liviu",
            "membership": false,
            "country": "RO"
          },
          "rating": 1910.1044,
          "deviation": 20
        },
        {
          "player": {
            "plid": 4090,
            "real_name": "David Milne",
            "membership": true,
            "country": "NZ"
          },
          "rating": 1551.7124,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 0,
      "expire_time": 1650892776238,
      "chngr": [
        2.8418925,
        -2.8418925
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685096,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 4152,
          "movetime": 1648489034864,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 2,
          "plid": 4090,
          "movetime": 1648512275850,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 3,
          "plid": 4152,
          "movetime": 1648528209593,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 4,
          "plid": 4090,
          "movetime": 1648548272850,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 5,
          "plid": 4152,
          "movetime": 1648549215439,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 6,
          "plid": 4090,
          "movetime": 1648600659194,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 7,
          "plid": 4152,
          "movetime": 1648615684046,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 8,
          "plid": 4090,
          "movetime": 1648639683659,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 9,
          "plid": 4152,
          "movetime": 1648645940370,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 10,
          "plid": 4090,
          "movetime": 1648689334559,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 11,
          "plid": 4152,
          "movetime": 1648701659742,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 12,
          "plid": 4090,
          "movetime": 1648802575039,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 13,
          "plid": 4152,
          "movetime": 1648835797001,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 14,
          "plid": 4090,
          "movetime": 1648862574552,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 15,
          "plid": 4152,
          "movetime": 1648876182931,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 16,
          "plid": 4090,
          "movetime": 1648892873026,
          "jmove": "ig",
          "dmove": "I7"
        },
        {
          "nmove": 17,
          "plid": 4152,
          "movetime": 1648985244264,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 18,
          "plid": 4090,
          "movetime": 1648988233407,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 19,
          "plid": 4152,
          "movetime": 1648988512496,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 20,
          "plid": 4090,
          "movetime": 1649061614341,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 21,
          "plid": 4152,
          "movetime": 1649081448327,
          "jmove": "ib",
          "dmove": "I2"
        },
        {
          "nmove": 22,
          "plid": 4090,
          "movetime": 1649121044389,
          "jmove": "ha",
          "dmove": "H1"
        },
        {
          "nmove": 23,
          "plid": 4152,
          "movetime": 1649132582929,
          "jmove": "bc",
          "dmove": "B3"
        },
        {
          "nmove": 24,
          "plid": 4090,
          "movetime": 1649208906232,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 25,
          "plid": 4152,
          "movetime": 1649221739700,
          "jmove": "fi",
          "dmove": "F9"
        },
        {
          "nmove": 26,
          "plid": 4090,
          "movetime": 1649290767676,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 27,
          "plid": 4152,
          "movetime": 1649305777793,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 28,
          "plid": 4090,
          "movetime": 1649378436938,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 29,
          "plid": 4152,
          "movetime": 1649390107909,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 30,
          "plid": 4090,
          "movetime": 1649469171638,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 31,
          "plid": 4152,
          "movetime": 1649487748605,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 32,
          "plid": 4090,
          "movetime": 1649552903123,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 33,
          "plid": 4152,
          "movetime": 1649572729735,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 34,
          "plid": 4090,
          "movetime": 1649643895312,
          "jmove": "ea",
          "dmove": "E1"
        },
        {
          "nmove": 35,
          "plid": 4152,
          "movetime": 1649651485845,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 36,
          "plid": 4090,
          "movetime": 1649727948350,
          "jmove": "bh",
          "dmove": "B8"
        },
        {
          "nmove": 37,
          "plid": 4152,
          "movetime": 1649738703422,
          "jmove": "af",
          "dmove": "A6"
        },
        {
          "nmove": 38,
          "plid": 4090,
          "movetime": 1649815817215,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 39,
          "plid": 4152,
          "movetime": 1649824758168,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 40,
          "plid": 4090,
          "movetime": 1650081511700,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 41,
          "plid": 4152,
          "movetime": 1650119413081,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 42,
          "plid": 4090,
          "movetime": 1650157843356,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 43,
          "plid": 4152,
          "movetime": 1650171344683,
          "jmove": "ag",
          "dmove": "A7"
        },
        {
          "nmove": 44,
          "plid": 4090,
          "movetime": 1650173187231,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 45,
          "plid": 4152,
          "movetime": 1650212508341,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 46,
          "plid": 4090,
          "movetime": 1650251498869,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 47,
          "plid": 4152,
          "movetime": 1650255432114,
          "jmove": "ie",
          "dmove": "I5"
        },
        {
          "nmove": 48,
          "plid": 4090,
          "movetime": 1650324559899,
          "jmove": "if",
          "dmove": "I6"
        },
        {
          "nmove": 49,
          "plid": 4152,
          "movetime": 1650337811346,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 50,
          "plid": 4090,
          "movetime": 1650458143286,
          "jmove": "gi",
          "dmove": "G9"
        },
        {
          "nmove": 51,
          "plid": 4152,
          "movetime": 1650470390112,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 52,
          "plid": 4090,
          "movetime": 1650515246050,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 53,
          "plid": 4152,
          "movetime": 1650517254182,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 54,
          "plid": 4090,
          "movetime": 1650593717387,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 55,
          "plid": 4152,
          "movetime": 1650606148650,
          "jmove": "bi",
          "dmove": "B9"
        },
        {
          "nmove": 56,
          "plid": 4090,
          "movetime": 1650622505862,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 57,
          "plid": 4152,
          "movetime": 1650645857115,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 58,
          "plid": 4090,
          "movetime": 1650677187372,
          "jmove": "fi",
          "dmove": "F9"
        },
        {
          "nmove": 59,
          "plid": 4152,
          "movetime": 1650684936772,
          "jmove": "ah",
          "dmove": "A8"
        },
        {
          "nmove": 60,
          "plid": 4090,
          "movetime": 1650718391861,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 61,
          "plid": 4152,
          "movetime": 1650727645801,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 62,
          "plid": 4090,
          "movetime": 1650766504285,
          "jmove": "ia",
          "dmove": "I1"
        },
        {
          "nmove": 63,
          "plid": 4152,
          "movetime": 1650784362862,
          "jmove": "ic",
          "dmove": "I3"
        },
        {
          "nmove": 64,
          "plid": 4090,
          "movetime": 1650857765608,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 65,
          "plid": 4152,
          "movetime": 1650889474581,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 66,
          "plid": 4090,
          "movetime": 1650892696583,
          "jmove": "score",
          "dmove": "Score"
        },
        {
          "nmove": 67,
          "plid": 4152,
          "movetime": 1650892776225,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302359,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 152553,
            "real_name": "pacmaniac",
            "membership": false,
            "country": "EU"
          },
          "rating": 1825.2876,
          "deviation": 31
        },
        {
          "player": {
            "plid": 4152,
            "real_name": "Liviu",
            "membership": false,
            "country": "RO"
          },
          "rating": 1910.1044,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 152553,
      "expire_time": 1650785664241,
      "chngr": [
        -18.475044,
        4.926678
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685099,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 152553,
          "movetime": 1648469055968,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 2,
          "plid": 4152,
          "movetime": 1648489051823,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 3,
          "plid": 152553,
          "movetime": 1648554893853,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 4,
          "plid": 4152,
          "movetime": 1648559315489,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 5,
          "plid": 152553,
          "movetime": 1648649778235,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 6,
          "plid": 4152,
          "movetime": 1648656119562,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 7,
          "plid": 152553,
          "movetime": 1648742284304,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 8,
          "plid": 4152,
          "movetime": 1648748366843,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 9,
          "plid": 152553,
          "movetime": 1648817793266,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 10,
          "plid": 4152,
          "movetime": 1648835839779,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 11,
          "plid": 152553,
          "movetime": 1648898303507,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 12,
          "plid": 4152,
          "movetime": 1648985249198,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 13,
          "plid": 152553,
          "movetime": 1649011615311,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 14,
          "plid": 4152,
          "movetime": 1649012291204,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 15,
          "plid": 152553,
          "movetime": 1649013606830,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 16,
          "plid": 4152,
          "movetime": 1649013814154,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 17,
          "plid": 152553,
          "movetime": 1649098724338,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 18,
          "plid": 4152,
          "movetime": 1649101297681,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 19,
          "plid": 152553,
          "movetime": 1649185918655,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 20,
          "plid": 4152,
          "movetime": 1649190978404,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 21,
          "plid": 152553,
          "movetime": 1649270753571,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 22,
          "plid": 4152,
          "movetime": 1649271259705,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 23,
          "plid": 152553,
          "movetime": 1649272586492,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 24,
          "plid": 4152,
          "movetime": 1649274608124,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 25,
          "plid": 152553,
          "movetime": 1649355361938,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 26,
          "plid": 4152,
          "movetime": 1649358630708,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 27,
          "plid": 152553,
          "movetime": 1649510233284,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 28,
          "plid": 4152,
          "movetime": 1649514862307,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 29,
          "plid": 152553,
          "movetime": 1649584793695,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 30,
          "plid": 4152,
          "movetime": 1649612608477,
          "jmove": "bb",
          "dmove": "B2"
        },
        {
          "nmove": 31,
          "plid": 152553,
          "movetime": 1649788347240,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 32,
          "plid": 4152,
          "movetime": 1649788857253,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 33,
          "plid": 152553,
          "movetime": 1649790037406,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 34,
          "plid": 4152,
          "movetime": 1649791692969,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 35,
          "plid": 152553,
          "movetime": 1649961055095,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 36,
          "plid": 4152,
          "movetime": 1649966398123,
          "jmove": "ie",
          "dmove": "I5"
        },
        {
          "nmove": 37,
          "plid": 152553,
          "movetime": 1650042082793,
          "jmove": "ha",
          "dmove": "H1"
        },
        {
          "nmove": 38,
          "plid": 4152,
          "movetime": 1650043463183,
          "jmove": "ag",
          "dmove": "A7"
        },
        {
          "nmove": 39,
          "plid": 152553,
          "movetime": 1650043515268,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 40,
          "plid": 4152,
          "movetime": 1650048716016,
          "jmove": "ig",
          "dmove": "I7"
        },
        {
          "nmove": 41,
          "plid": 152553,
          "movetime": 1650116907853,
          "jmove": "ic",
          "dmove": "I3"
        },
        {
          "nmove": 42,
          "plid": 4152,
          "movetime": 1650119425563,
          "jmove": "id",
          "dmove": "I4"
        },
        {
          "nmove": 43,
          "plid": 152553,
          "movetime": 1650218052676,
          "jmove": "bh",
          "dmove": "B8"
        },
        {
          "nmove": 44,
          "plid": 4152,
          "movetime": 1650218573525,
          "jmove": "ah",
          "dmove": "A8"
        },
        {
          "nmove": 45,
          "plid": 152553,
          "movetime": 1650219529264,
          "jmove": "ih",
          "dmove": "I8"
        },
        {
          "nmove": 46,
          "plid": 4152,
          "movetime": 1650219919675,
          "jmove": "bi",
          "dmove": "B9"
        },
        {
          "nmove": 47,
          "plid": 152553,
          "movetime": 1650277535137,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 48,
          "plid": 4152,
          "movetime": 1650301194024,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 49,
          "plid": 152553,
          "movetime": 1650307042519,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 50,
          "plid": 4152,
          "movetime": 1650307788575,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 51,
          "plid": 152553,
          "movetime": 1650308436306,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 52,
          "plid": 4152,
          "movetime": 1650308476542,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 53,
          "plid": 152553,
          "movetime": 1650308545219,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 54,
          "plid": 4152,
          "movetime": 1650308861482,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 55,
          "plid": 152553,
          "movetime": 1650391523966,
          "jmove": "ga",
          "dmove": "G1"
        },
        {
          "nmove": 56,
          "plid": 4152,
          "movetime": 1650392703682,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 57,
          "plid": 152553,
          "movetime": 1650394473901,
          "jmove": "af",
          "dmove": "A6"
        },
        {
          "nmove": 58,
          "plid": 4152,
          "movetime": 1650394993237,
          "jmove": "ae",
          "dmove": "A5"
        },
        {
          "nmove": 59,
          "plid": 152553,
          "movetime": 1650478825562,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 60,
          "plid": 4152,
          "movetime": 1650479157139,
          "jmove": "ea",
          "dmove": "E1"
        },
        {
          "nmove": 61,
          "plid": 152553,
          "movetime": 1650565777310,
          "jmove": "fa",
          "dmove": "F1"
        },
        {
          "nmove": 62,
          "plid": 4152,
          "movetime": 1650567947980,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 63,
          "plid": 152553,
          "movetime": 1650568473608,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 64,
          "plid": 4152,
          "movetime": 1650570379799,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 65,
          "plid": 152553,
          "movetime": 1650738912126,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 66,
          "plid": 4152,
          "movetime": 1650739372760,
          "jmove": "ib",
          "dmove": "I2"
        },
        {
          "nmove": 67,
          "plid": 152553,
          "movetime": 1650741107274,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 68,
          "plid": 4152,
          "movetime": 1650784338319,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 69,
          "plid": 152553,
          "movetime": 1650785003221,
          "jmove": "fi",
          "dmove": "F9"
        },
        {
          "nmove": 70,
          "plid": 4152,
          "movetime": 1650785188121,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 71,
          "plid": 152553,
          "movetime": 1650785664226,
          "jmove": "resign",
          "dmove": "resign"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302360,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 4152,
            "real_name": "Liviu",
            "membership": false,
            "country": "RO"
          },
          "rating": 1910.1044,
          "deviation": 20
        },
        {
          "player": {
            "plid": 144760,
            "real_name": "galispiar",
            "membership": false,
            "country": "JP"
          },
          "rating": 1021.5246,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 144760,
      "expire_time": 1649749683526,
      "chngr": [
        1.297848,
        -3.569082
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685101,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 4152,
          "movetime": 1648489037564,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 2,
          "plid": 144760,
          "movetime": 1649154639517,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 3,
          "plid": 4152,
          "movetime": 1649162541603,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 4,
          "plid": 144760,
          "movetime": 1649401300323,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 5,
          "plid": 4152,
          "movetime": 1649442024746,
          "jmove": "dg",
          "dmove": "D7"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        223200000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302361,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 22709,
            "real_name": "Thierry Pertuy",
            "membership": false,
            "country": "FR"
          },
          "rating": 1756.0692,
          "deviation": 20
        },
        {
          "player": {
            "plid": 21042,
            "real_name": "drToma",
            "membership": false,
            "country": "RO"
          },
          "rating": 1707.7354,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 0,
      "expire_time": 1651162202230,
      "chngr": [
        11.104538,
        -11.104538
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685104,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 22709,
          "movetime": 1648500163060,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 2,
          "plid": 21042,
          "movetime": 1648563301231,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 3,
          "plid": 22709,
          "movetime": 1648571264451,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 4,
          "plid": 21042,
          "movetime": 1648734741730,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 5,
          "plid": 22709,
          "movetime": 1648744338428,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 6,
          "plid": 21042,
          "movetime": 1648919592793,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 7,
          "plid": 22709,
          "movetime": 1648938873564,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 8,
          "plid": 21042,
          "movetime": 1649015102448,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 9,
          "plid": 22709,
          "movetime": 1649017889479,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 10,
          "plid": 21042,
          "movetime": 1649088514073,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 11,
          "plid": 22709,
          "movetime": 1649091192384,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 12,
          "plid": 21042,
          "movetime": 1649093631985,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 13,
          "plid": 22709,
          "movetime": 1649102188579,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 14,
          "plid": 21042,
          "movetime": 1649169809320,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 15,
          "plid": 22709,
          "movetime": 1649173805940,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 16,
          "plid": 21042,
          "movetime": 1649326150688,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 17,
          "plid": 22709,
          "movetime": 1649329786811,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 18,
          "plid": 21042,
          "movetime": 1649352338043,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 19,
          "plid": 22709,
          "movetime": 1649358389561,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 20,
          "plid": 21042,
          "movetime": 1649425552869,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 21,
          "plid": 22709,
          "movetime": 1649428682204,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 22,
          "plid": 21042,
          "movetime": 1649593843881,
          "jmove": "if",
          "dmove": "I6"
        },
        {
          "nmove": 23,
          "plid": 22709,
          "movetime": 1649619724047,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 24,
          "plid": 21042,
          "movetime": 1649670688245,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 25,
          "plid": 22709,
          "movetime": 1649674078090,
          "jmove": "ih",
          "dmove": "I8"
        },
        {
          "nmove": 26,
          "plid": 21042,
          "movetime": 1649674463664,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 27,
          "plid": 22709,
          "movetime": 1649683198581,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 28,
          "plid": 21042,
          "movetime": 1649688348265,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 29,
          "plid": 22709,
          "movetime": 1649704062749,
          "jmove": "ha",
          "dmove": "H1"
        },
        {
          "nmove": 30,
          "plid": 21042,
          "movetime": 1649773770480,
          "jmove": "ib",
          "dmove": "I2"
        },
        {
          "nmove": 31,
          "plid": 22709,
          "movetime": 1649783012335,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 32,
          "plid": 21042,
          "movetime": 1649859929709,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 33,
          "plid": 22709,
          "movetime": 1649860315471,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 34,
          "plid": 21042,
          "movetime": 1649863558573,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 35,
          "plid": 22709,
          "movetime": 1649866265069,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 36,
          "plid": 21042,
          "movetime": 1649871482580,
          "jmove": "ae",
          "dmove": "A5"
        },
        {
          "nmove": 37,
          "plid": 22709,
          "movetime": 1649874635227,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 38,
          "plid": 21042,
          "movetime": 1649874782835,
          "jmove": "af",
          "dmove": "A6"
        },
        {
          "nmove": 39,
          "plid": 22709,
          "movetime": 1649877886896,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 40,
          "plid": 21042,
          "movetime": 1649953579001,
          "jmove": "ig",
          "dmove": "I7"
        },
        {
          "nmove": 41,
          "plid": 22709,
          "movetime": 1649954176832,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 42,
          "plid": 21042,
          "movetime": 1649959814394,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 43,
          "plid": 22709,
          "movetime": 1649961037938,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 44,
          "plid": 21042,
          "movetime": 1649961330317,
          "jmove": "bi",
          "dmove": "B9"
        },
        {
          "nmove": 45,
          "plid": 22709,
          "movetime": 1649962251662,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 46,
          "plid": 21042,
          "movetime": 1650238094759,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 47,
          "plid": 22709,
          "movetime": 1650266671194,
          "jmove": "ga",
          "dmove": "G1"
        },
        {
          "nmove": 48,
          "plid": 21042,
          "movetime": 1650463300203,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 49,
          "plid": 22709,
          "movetime": 1650468670226,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 50,
          "plid": 21042,
          "movetime": 1650711184392,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 51,
          "plid": 22709,
          "movetime": 1650843578456,
          "jmove": "score",
          "dmove": "Score"
        },
        {
          "nmove": 52,
          "plid": 21042,
          "movetime": 1651162202225,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        543600000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302362,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 21042,
            "real_name": "drToma",
            "membership": false,
            "country": "RO"
          },
          "rating": 1707.7354,
          "deviation": 20
        },
        {
          "player": {
            "plid": 1017,
            "real_name": "Elisa Kabiljo",
            "membership": false,
            "country": "RS"
          },
          "rating": 1698.1548,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 0,
      "expire_time": 1651351027595,
      "chngr": [
        -11.703007,
        11.703007
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685107,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 21042,
          "movetime": 1648467128668,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 2,
          "plid": 1017,
          "movetime": 1648487189478,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 3,
          "plid": 21042,
          "movetime": 1648490691311,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 4,
          "plid": 1017,
          "movetime": 1648506655483,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 5,
          "plid": 21042,
          "movetime": 1648563305241,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 6,
          "plid": 1017,
          "movetime": 1648576069009,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 7,
          "plid": 21042,
          "movetime": 1648734774404,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 8,
          "plid": 1017,
          "movetime": 1648754586868,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 9,
          "plid": 21042,
          "movetime": 1649425529768,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 10,
          "plid": 1017,
          "movetime": 1649453525557,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 11,
          "plid": 21042,
          "movetime": 1649593824591,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 12,
          "plid": 1017,
          "movetime": 1649615515655,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 13,
          "plid": 21042,
          "movetime": 1649616932063,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 14,
          "plid": 1017,
          "movetime": 1649626076061,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 15,
          "plid": 21042,
          "movetime": 1649670684134,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 16,
          "plid": 1017,
          "movetime": 1649714580075,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 17,
          "plid": 21042,
          "movetime": 1649773757627,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 18,
          "plid": 1017,
          "movetime": 1649800968720,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 19,
          "plid": 21042,
          "movetime": 1649859910417,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 20,
          "plid": 1017,
          "movetime": 1649862949916,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 21,
          "plid": 21042,
          "movetime": 1649863554372,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 22,
          "plid": 1017,
          "movetime": 1649888385552,
          "jmove": "ac",
          "dmove": "A3"
        },
        {
          "nmove": 23,
          "plid": 21042,
          "movetime": 1649953555687,
          "jmove": "ae",
          "dmove": "A5"
        },
        {
          "nmove": 24,
          "plid": 1017,
          "movetime": 1649968311741,
          "jmove": "bb",
          "dmove": "B2"
        },
        {
          "nmove": 25,
          "plid": 21042,
          "movetime": 1650750280537,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 26,
          "plid": 1017,
          "movetime": 1650779433428,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 27,
          "plid": 21042,
          "movetime": 1650797906688,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 28,
          "plid": 1017,
          "movetime": 1650820121081,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 29,
          "plid": 21042,
          "movetime": 1650826475276,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 30,
          "plid": 1017,
          "movetime": 1650865835645,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 31,
          "plid": 21042,
          "movetime": 1651162182782,
          "jmove": "id",
          "dmove": "I4"
        },
        {
          "nmove": 32,
          "plid": 1017,
          "movetime": 1651167119135,
          "jmove": "ic",
          "dmove": "I3"
        },
        {
          "nmove": 33,
          "plid": 21042,
          "movetime": 1651168480531,
          "jmove": "ie",
          "dmove": "I5"
        },
        {
          "nmove": 34,
          "plid": 1017,
          "movetime": 1651180275730,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 35,
          "plid": 21042,
          "movetime": 1651255189482,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 36,
          "plid": 1017,
          "movetime": 1651256763684,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 37,
          "plid": 21042,
          "movetime": 1651341931316,
          "jmove": "scoregg",
          "dmove": "Score"
        },
        {
          "nmove": 38,
          "plid": 1017,
          "movetime": 1651351027590,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        496800000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302363,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 8262,
            "real_name": "Zandor",
            "membership": false,
            "country": "AT"
          },
          "rating": 1716.0134,
          "deviation": 20
        },
        {
          "player": {
            "plid": 21042,
            "real_name": "drToma",
            "membership": false,
            "country": "RO"
          },
          "rating": 1707.7354,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 0,
      "expire_time": 1649959823967,
      "chngr": [
        12.171455,
        -12.171455
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685109,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 8262,
          "movetime": 1648478776977,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 2,
          "plid": 21042,
          "movetime": 1648482652545,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 3,
          "plid": 8262,
          "movetime": 1648511110211,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 4,
          "plid": 21042,
          "movetime": 1648563315518,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 5,
          "plid": 8262,
          "movetime": 1648567564642,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 6,
          "plid": 21042,
          "movetime": 1648734736094,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 7,
          "plid": 8262,
          "movetime": 1648838727512,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 8,
          "plid": 21042,
          "movetime": 1648844432535,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 9,
          "plid": 8262,
          "movetime": 1648847619319,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 10,
          "plid": 21042,
          "movetime": 1648919685616,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 11,
          "plid": 8262,
          "movetime": 1648922732293,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 12,
          "plid": 21042,
          "movetime": 1648936522177,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 13,
          "plid": 8262,
          "movetime": 1649096021750,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 14,
          "plid": 21042,
          "movetime": 1649097457158,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 15,
          "plid": 8262,
          "movetime": 1649108167756,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 16,
          "plid": 21042,
          "movetime": 1649169812451,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 17,
          "plid": 8262,
          "movetime": 1649346305384,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 18,
          "plid": 21042,
          "movetime": 1649352345030,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 19,
          "plid": 8262,
          "movetime": 1649443842698,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 20,
          "plid": 21042,
          "movetime": 1649593867247,
          "jmove": "ba",
          "dmove": "B1"
        },
        {
          "nmove": 21,
          "plid": 8262,
          "movetime": 1649631159878,
          "jmove": "ea",
          "dmove": "E1"
        },
        {
          "nmove": 22,
          "plid": 21042,
          "movetime": 1649670732629,
          "jmove": "bc",
          "dmove": "B3"
        },
        {
          "nmove": 23,
          "plid": 8262,
          "movetime": 1649688259181,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 24,
          "plid": 21042,
          "movetime": 1649688352002,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 25,
          "plid": 8262,
          "movetime": 1649709203863,
          "jmove": "fi",
          "dmove": "F9"
        },
        {
          "nmove": 26,
          "plid": 21042,
          "movetime": 1649773778115,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 27,
          "plid": 8262,
          "movetime": 1649862302246,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 28,
          "plid": 21042,
          "movetime": 1649863568472,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 29,
          "plid": 8262,
          "movetime": 1649865043769,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 30,
          "plid": 21042,
          "movetime": 1649871474328,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 31,
          "plid": 8262,
          "movetime": 1649937574304,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 32,
          "plid": 21042,
          "movetime": 1649953590688,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 33,
          "plid": 8262,
          "movetime": 1649956362823,
          "jmove": "score",
          "dmove": "Score"
        },
        {
          "nmove": 34,
          "plid": 21042,
          "movetime": 1649959823963,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302364,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 21042,
            "real_name": "drToma",
            "membership": false,
            "country": "RO"
          },
          "rating": 1707.7354,
          "deviation": 20
        },
        {
          "player": {
            "plid": 44616,
            "real_name": "nullptr",
            "membership": false,
            "country": "US"
          },
          "rating": 1737.2621,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 0,
      "expire_time": 1652147071145,
      "chngr": [
        -12.251296,
        12.251296
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685111,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 21042,
          "movetime": 1648467136742,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 2,
          "plid": 44616,
          "movetime": 1648516112126,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 3,
          "plid": 21042,
          "movetime": 1648563341233,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 4,
          "plid": 44616,
          "movetime": 1648603584792,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 5,
          "plid": 21042,
          "movetime": 1648734830801,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 6,
          "plid": 44616,
          "movetime": 1648775760173,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 7,
          "plid": 21042,
          "movetime": 1648844356097,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 8,
          "plid": 44616,
          "movetime": 1648856929689,
          "jmove": "bb",
          "dmove": "B2"
        },
        {
          "nmove": 9,
          "plid": 21042,
          "movetime": 1648919690522,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 10,
          "plid": 44616,
          "movetime": 1648951906911,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 11,
          "plid": 21042,
          "movetime": 1649088504625,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 12,
          "plid": 44616,
          "movetime": 1649129386564,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 13,
          "plid": 21042,
          "movetime": 1649169831982,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 14,
          "plid": 44616,
          "movetime": 1649206968944,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 15,
          "plid": 21042,
          "movetime": 1649326168637,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 16,
          "plid": 44616,
          "movetime": 1649359903467,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 17,
          "plid": 21042,
          "movetime": 1649425566630,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 18,
          "plid": 44616,
          "movetime": 1649430016737,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 19,
          "plid": 21042,
          "movetime": 1649593855519,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 20,
          "plid": 44616,
          "movetime": 1649638650084,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 21,
          "plid": 21042,
          "movetime": 1649670728952,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 22,
          "plid": 44616,
          "movetime": 1649724280407,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 23,
          "plid": 21042,
          "movetime": 1649773789162,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 24,
          "plid": 44616,
          "movetime": 1649895597729,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 25,
          "plid": 21042,
          "movetime": 1649953583536,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 26,
          "plid": 44616,
          "movetime": 1649980035166,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 27,
          "plid": 21042,
          "movetime": 1650238111300,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 28,
          "plid": 44616,
          "movetime": 1650331114208,
          "jmove": "fi",
          "dmove": "F9"
        },
        {
          "nmove": 29,
          "plid": 21042,
          "movetime": 1650463415795,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 30,
          "plid": 44616,
          "movetime": 1650501540334,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 31,
          "plid": 21042,
          "movetime": 1650711190100,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 32,
          "plid": 44616,
          "movetime": 1650728160173,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 33,
          "plid": 21042,
          "movetime": 1650797930739,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 34,
          "plid": 44616,
          "movetime": 1650809766427,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 35,
          "plid": 21042,
          "movetime": 1650826496005,
          "jmove": "ih",
          "dmove": "I8"
        },
        {
          "nmove": 36,
          "plid": 44616,
          "movetime": 1650942354432,
          "jmove": "gi",
          "dmove": "G9"
        },
        {
          "nmove": 37,
          "plid": 21042,
          "movetime": 1651162236866,
          "jmove": "ba",
          "dmove": "B1"
        },
        {
          "nmove": 38,
          "plid": 44616,
          "movetime": 1651197858672,
          "jmove": "aa",
          "dmove": "A1"
        },
        {
          "nmove": 39,
          "plid": 21042,
          "movetime": 1651255209294,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 40,
          "plid": 44616,
          "movetime": 1651285099644,
          "jmove": "bc",
          "dmove": "B3"
        },
        {
          "nmove": 41,
          "plid": 21042,
          "movetime": 1651341946581,
          "jmove": "ba",
          "dmove": "B1"
        },
        {
          "nmove": 42,
          "plid": 44616,
          "movetime": 1651364982953,
          "jmove": "ab",
          "dmove": "A2"
        },
        {
          "nmove": 43,
          "plid": 21042,
          "movetime": 1651500827512,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 44,
          "plid": 44616,
          "movetime": 1651632781911,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 45,
          "plid": 21042,
          "movetime": 1651765409833,
          "jmove": "ig",
          "dmove": "I7"
        },
        {
          "nmove": 46,
          "plid": 44616,
          "movetime": 1651795694517,
          "jmove": "hi",
          "dmove": "H9"
        },
        {
          "nmove": 47,
          "plid": 21042,
          "movetime": 1651992752510,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 48,
          "plid": 44616,
          "movetime": 1652056177135,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 49,
          "plid": 21042,
          "movetime": 1652118835240,
          "jmove": "score",
          "dmove": "Score"
        },
        {
          "nmove": 50,
          "plid": 44616,
          "movetime": 1652147071139,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302365,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 4090,
            "real_name": "David Milne",
            "membership": true,
            "country": "NZ"
          },
          "rating": 1551.7124,
          "deviation": 20
        },
        {
          "player": {
            "plid": 21042,
            "real_name": "drToma",
            "membership": false,
            "country": "RO"
          },
          "rating": 1707.7354,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 0,
      "expire_time": 1651834716871,
      "chngr": [
        -7.467581,
        7.467581
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685113,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 4090,
          "movetime": 1648456005305,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 2,
          "plid": 21042,
          "movetime": 1648467151150,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 3,
          "plid": 4090,
          "movetime": 1648512250433,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 4,
          "plid": 21042,
          "movetime": 1648563337581,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 5,
          "plid": 4090,
          "movetime": 1648600778745,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 6,
          "plid": 21042,
          "movetime": 1648735455539,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 7,
          "plid": 4090,
          "movetime": 1648802701074,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 8,
          "plid": 21042,
          "movetime": 1648919627794,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 9,
          "plid": 4090,
          "movetime": 1648960035671,
          "jmove": "fi",
          "dmove": "F9"
        },
        {
          "nmove": 10,
          "plid": 21042,
          "movetime": 1649015174597,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 11,
          "plid": 4090,
          "movetime": 1649061793728,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 12,
          "plid": 21042,
          "movetime": 1649088524374,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 13,
          "plid": 4090,
          "movetime": 1649121066398,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 14,
          "plid": 21042,
          "movetime": 1649169821189,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 15,
          "plid": 4090,
          "movetime": 1649209072940,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 16,
          "plid": 21042,
          "movetime": 1649326178680,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 17,
          "plid": 4090,
          "movetime": 1649378558321,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 18,
          "plid": 21042,
          "movetime": 1649425569986,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 19,
          "plid": 4090,
          "movetime": 1649469230563,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 20,
          "plid": 21042,
          "movetime": 1649593878759,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 21,
          "plid": 4090,
          "movetime": 1649644006872,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 22,
          "plid": 21042,
          "movetime": 1649670778989,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 23,
          "plid": 4090,
          "movetime": 1649728036753,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 24,
          "plid": 21042,
          "movetime": 1649773795210,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 25,
          "plid": 4090,
          "movetime": 1649815921620,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 26,
          "plid": 21042,
          "movetime": 1649859959135,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 27,
          "plid": 4090,
          "movetime": 1650082223899,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 28,
          "plid": 21042,
          "movetime": 1650238121096,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 29,
          "plid": 4090,
          "movetime": 1650251660860,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 30,
          "plid": 21042,
          "movetime": 1650385539482,
          "jmove": "if",
          "dmove": "I6"
        },
        {
          "nmove": 31,
          "plid": 4090,
          "movetime": 1650458258818,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 32,
          "plid": 21042,
          "movetime": 1650463437575,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 33,
          "plid": 4090,
          "movetime": 1650515204086,
          "jmove": "ha",
          "dmove": "H1"
        },
        {
          "nmove": 34,
          "plid": 21042,
          "movetime": 1650711212064,
          "jmove": "ib",
          "dmove": "I2"
        },
        {
          "nmove": 35,
          "plid": 4090,
          "movetime": 1650718566127,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 36,
          "plid": 21042,
          "movetime": 1650797951750,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 37,
          "plid": 4090,
          "movetime": 1650857892642,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 38,
          "plid": 21042,
          "movetime": 1651162219915,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 39,
          "plid": 4090,
          "movetime": 1651201457355,
          "jmove": "ba",
          "dmove": "B1"
        },
        {
          "nmove": 40,
          "plid": 21042,
          "movetime": 1651255203990,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 41,
          "plid": 4090,
          "movetime": 1651289019297,
          "jmove": "ab",
          "dmove": "A2"
        },
        {
          "nmove": 42,
          "plid": 21042,
          "movetime": 1651341942268,
          "jmove": "hi",
          "dmove": "H9"
        },
        {
          "nmove": 43,
          "plid": 4090,
          "movetime": 1651375218294,
          "jmove": "gi",
          "dmove": "G9"
        },
        {
          "nmove": 44,
          "plid": 21042,
          "movetime": 1651500823481,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 45,
          "plid": 4090,
          "movetime": 1651545199304,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 46,
          "plid": 21042,
          "movetime": 1651589342369,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 47,
          "plid": 4090,
          "movetime": 1651621151068,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 48,
          "plid": 21042,
          "movetime": 1651765384649,
          "jmove": "scorehc",
          "dmove": "Score"
        },
        {
          "nmove": 49,
          "plid": 4090,
          "movetime": 1651834716783,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        950400000,
        849600000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302366,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 21042,
            "real_name": "drToma",
            "membership": false,
            "country": "RO"
          },
          "rating": 1707.7354,
          "deviation": 20
        },
        {
          "player": {
            "plid": 152553,
            "real_name": "pacmaniac",
            "membership": false,
            "country": "EU"
          },
          "rating": 1825.2876,
          "deviation": 31
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 0,
      "expire_time": 1652118025108,
      "chngr": [
        -8.308454,
        28.664165
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685115,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 21042,
          "movetime": 1648467143641,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 2,
          "plid": 152553,
          "movetime": 1648469180605,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 3,
          "plid": 21042,
          "movetime": 1648482647966,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 4,
          "plid": 152553,
          "movetime": 1648554857150,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 5,
          "plid": 21042,
          "movetime": 1648563356807,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 6,
          "plid": 152553,
          "movetime": 1648649816649,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 7,
          "plid": 21042,
          "movetime": 1648734836000,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 8,
          "plid": 152553,
          "movetime": 1648742472417,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 9,
          "plid": 21042,
          "movetime": 1648757589616,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 10,
          "plid": 152553,
          "movetime": 1648817852624,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 11,
          "plid": 21042,
          "movetime": 1649088493589,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 12,
          "plid": 152553,
          "movetime": 1649098894512,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 13,
          "plid": 21042,
          "movetime": 1649169805708,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 14,
          "plid": 152553,
          "movetime": 1649186188778,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 15,
          "plid": 21042,
          "movetime": 1649326142913,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 16,
          "plid": 152553,
          "movetime": 1649355599483,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 17,
          "plid": 21042,
          "movetime": 1649425537363,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 18,
          "plid": 152553,
          "movetime": 1649510340515,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 19,
          "plid": 21042,
          "movetime": 1649593888190,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 20,
          "plid": 152553,
          "movetime": 1649788278199,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 21,
          "plid": 21042,
          "movetime": 1649859933712,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 22,
          "plid": 152553,
          "movetime": 1649961097099,
          "jmove": "ie",
          "dmove": "I5"
        },
        {
          "nmove": 23,
          "plid": 21042,
          "movetime": 1649961333598,
          "jmove": "id",
          "dmove": "I4"
        },
        {
          "nmove": 24,
          "plid": 152553,
          "movetime": 1649962848035,
          "jmove": "if",
          "dmove": "I6"
        },
        {
          "nmove": 25,
          "plid": 21042,
          "movetime": 1650238099658,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 26,
          "plid": 152553,
          "movetime": 1650277605204,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 27,
          "plid": 21042,
          "movetime": 1650385500268,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 28,
          "plid": 152553,
          "movetime": 1650391695981,
          "jmove": "bb",
          "dmove": "B2"
        },
        {
          "nmove": 29,
          "plid": 21042,
          "movetime": 1650463425951,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 30,
          "plid": 152553,
          "movetime": 1650478921204,
          "jmove": "ba",
          "dmove": "B1"
        },
        {
          "nmove": 31,
          "plid": 21042,
          "movetime": 1650711206327,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 32,
          "plid": 152553,
          "movetime": 1650739144196,
          "jmove": "fi",
          "dmove": "F9"
        },
        {
          "nmove": 33,
          "plid": 21042,
          "movetime": 1650797945674,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 34,
          "plid": 152553,
          "movetime": 1650824966118,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 35,
          "plid": 21042,
          "movetime": 1650826505526,
          "jmove": "bh",
          "dmove": "B8"
        },
        {
          "nmove": 36,
          "plid": 152553,
          "movetime": 1650908928176,
          "jmove": "ah",
          "dmove": "A8"
        },
        {
          "nmove": 37,
          "plid": 21042,
          "movetime": 1651162229161,
          "jmove": "ag",
          "dmove": "A7"
        },
        {
          "nmove": 38,
          "plid": 152553,
          "movetime": 1651167817400,
          "jmove": "af",
          "dmove": "A6"
        },
        {
          "nmove": 39,
          "plid": 21042,
          "movetime": 1651168488482,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 40,
          "plid": 152553,
          "movetime": 1651170027842,
          "jmove": "ih",
          "dmove": "I8"
        },
        {
          "nmove": 41,
          "plid": 21042,
          "movetime": 1651171131571,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 42,
          "plid": 152553,
          "movetime": 1651338453881,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 43,
          "plid": 21042,
          "movetime": 1651341950708,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 44,
          "plid": 152553,
          "movetime": 1651344212653,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 45,
          "plid": 21042,
          "movetime": 1651351489983,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 46,
          "plid": 152553,
          "movetime": 1651385046209,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 47,
          "plid": 21042,
          "movetime": 1651500837211,
          "jmove": "bi",
          "dmove": "B9"
        },
        {
          "nmove": 48,
          "plid": 152553,
          "movetime": 1651561380014,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 49,
          "plid": 21042,
          "movetime": 1651589348612,
          "jmove": "ai",
          "dmove": "A9"
        },
        {
          "nmove": 50,
          "plid": 152553,
          "movetime": 1651598930742,
          "jmove": "ag",
          "dmove": "A7"
        },
        {
          "nmove": 51,
          "plid": 21042,
          "movetime": 1651765370785,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 52,
          "plid": 152553,
          "movetime": 1651773895406,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 53,
          "plid": 21042,
          "movetime": 1651992744862,
          "jmove": "score",
          "dmove": "Score"
        },
        {
          "nmove": 54,
          "plid": 152553,
          "movetime": 1652118025103,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        828000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302367,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 144760,
            "real_name": "galispiar",
            "membership": false,
            "country": "JP"
          },
          "rating": 1021.5246,
          "deviation": 20
        },
        {
          "player": {
            "plid": 21042,
            "real_name": "drToma",
            "membership": false,
            "country": "RO"
          },
          "rating": 1707.7354,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 144760,
      "expire_time": 1649749679930,
      "chngr": [
        -12.667999,
        4.1534424
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685118,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 144760,
          "movetime": 1649154059763,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 2,
          "plid": 21042,
          "movetime": 1649169837726,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 3,
          "plid": 144760,
          "movetime": 1649401173726,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 4,
          "plid": 21042,
          "movetime": 1649425751847,
          "jmove": "dd",
          "dmove": "D4"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        194400000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302368,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 1017,
            "real_name": "Elisa Kabiljo",
            "membership": false,
            "country": "RS"
          },
          "rating": 1698.1548,
          "deviation": 20
        },
        {
          "player": {
            "plid": 22709,
            "real_name": "Thierry Pertuy",
            "membership": false,
            "country": "FR"
          },
          "rating": 1756.0692,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 0,
      "expire_time": 1649667526103,
      "chngr": [
        -10.001511,
        10.001511
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685125,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 1017,
          "movetime": 1648457764110,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 2,
          "plid": 22709,
          "movetime": 1648500252305,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 3,
          "plid": 1017,
          "movetime": 1648506673940,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 4,
          "plid": 22709,
          "movetime": 1648507308581,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 5,
          "plid": 1017,
          "movetime": 1648534598900,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 6,
          "plid": 22709,
          "movetime": 1648539865407,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 7,
          "plid": 1017,
          "movetime": 1648576012965,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 8,
          "plid": 22709,
          "movetime": 1648594912343,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 9,
          "plid": 1017,
          "movetime": 1648618963877,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 10,
          "plid": 22709,
          "movetime": 1648626455654,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 11,
          "plid": 1017,
          "movetime": 1648659171884,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 12,
          "plid": 22709,
          "movetime": 1648663026774,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 13,
          "plid": 1017,
          "movetime": 1648679590239,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 14,
          "plid": 22709,
          "movetime": 1648727287375,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 15,
          "plid": 1017,
          "movetime": 1648754563939,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 16,
          "plid": 22709,
          "movetime": 1648757012442,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 17,
          "plid": 1017,
          "movetime": 1648765481499,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 18,
          "plid": 22709,
          "movetime": 1648938231580,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 19,
          "plid": 1017,
          "movetime": 1648963724418,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 20,
          "plid": 22709,
          "movetime": 1648969206864,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 21,
          "plid": 1017,
          "movetime": 1648980369126,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 22,
          "plid": 22709,
          "movetime": 1648983095399,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 23,
          "plid": 1017,
          "movetime": 1649002454607,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 24,
          "plid": 22709,
          "movetime": 1649010321346,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 25,
          "plid": 1017,
          "movetime": 1649024631257,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 26,
          "plid": 22709,
          "movetime": 1649053894106,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 27,
          "plid": 1017,
          "movetime": 1649054057466,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 28,
          "plid": 22709,
          "movetime": 1649054548321,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 29,
          "plid": 1017,
          "movetime": 1649097421219,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 30,
          "plid": 22709,
          "movetime": 1649106447620,
          "jmove": "ie",
          "dmove": "I5"
        },
        {
          "nmove": 31,
          "plid": 1017,
          "movetime": 1649135046772,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 32,
          "plid": 22709,
          "movetime": 1649139095910,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 33,
          "plid": 1017,
          "movetime": 1649182057878,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 34,
          "plid": 22709,
          "movetime": 1649189044568,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 35,
          "plid": 1017,
          "movetime": 1649191068808,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 36,
          "plid": 22709,
          "movetime": 1649195294677,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 37,
          "plid": 1017,
          "movetime": 1649224982232,
          "jmove": "ea",
          "dmove": "E1"
        },
        {
          "nmove": 38,
          "plid": 22709,
          "movetime": 1649227599089,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 39,
          "plid": 1017,
          "movetime": 1649264388540,
          "jmove": "bh",
          "dmove": "B8"
        },
        {
          "nmove": 40,
          "plid": 22709,
          "movetime": 1649265825531,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 41,
          "plid": 1017,
          "movetime": 1649279197160,
          "jmove": "fa",
          "dmove": "F1"
        },
        {
          "nmove": 42,
          "plid": 22709,
          "movetime": 1649280267946,
          "jmove": "ah",
          "dmove": "A8"
        },
        {
          "nmove": 43,
          "plid": 1017,
          "movetime": 1649331802597,
          "jmove": "id",
          "dmove": "I4"
        },
        {
          "nmove": 44,
          "plid": 22709,
          "movetime": 1649335272158,
          "jmove": "if",
          "dmove": "I6"
        },
        {
          "nmove": 45,
          "plid": 1017,
          "movetime": 1649367781688,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 46,
          "plid": 22709,
          "movetime": 1649370890303,
          "jmove": "fi",
          "dmove": "F9"
        },
        {
          "nmove": 47,
          "plid": 1017,
          "movetime": 1649372329622,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 48,
          "plid": 22709,
          "movetime": 1649387400567,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 49,
          "plid": 1017,
          "movetime": 1649453406149,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 50,
          "plid": 22709,
          "movetime": 1649487407839,
          "jmove": "ih",
          "dmove": "I8"
        },
        {
          "nmove": 51,
          "plid": 1017,
          "movetime": 1649511092940,
          "jmove": "hi",
          "dmove": "H9"
        },
        {
          "nmove": 52,
          "plid": 22709,
          "movetime": 1649511632509,
          "jmove": "gi",
          "dmove": "G9"
        },
        {
          "nmove": 53,
          "plid": 1017,
          "movetime": 1649532132422,
          "jmove": "bi",
          "dmove": "B9"
        },
        {
          "nmove": 54,
          "plid": 22709,
          "movetime": 1649532362173,
          "jmove": "ag",
          "dmove": "A7"
        },
        {
          "nmove": 55,
          "plid": 1017,
          "movetime": 1649532556598,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 56,
          "plid": 22709,
          "movetime": 1649534805246,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 57,
          "plid": 1017,
          "movetime": 1649567762971,
          "jmove": "scoreed",
          "dmove": "Score"
        },
        {
          "nmove": 58,
          "plid": 22709,
          "movetime": 1649568194860,
          "jmove": "scorehied",
          "dmove": "Score"
        },
        {
          "nmove": 59,
          "plid": 1017,
          "movetime": 1649610006669,
          "jmove": "scoreed",
          "dmove": "Score"
        },
        {
          "nmove": 60,
          "plid": 22709,
          "movetime": 1649619694486,
          "jmove": "scorehhed",
          "dmove": "Score"
        },
        {
          "nmove": 61,
          "plid": 1017,
          "movetime": 1649626140523,
          "jmove": "scoreed",
          "dmove": "Score"
        },
        {
          "nmove": 62,
          "plid": 22709,
          "movetime": 1649664920386,
          "jmove": "scorehied",
          "dmove": "Score"
        },
        {
          "nmove": 63,
          "plid": 1017,
          "movetime": 1649666234790,
          "jmove": "scoreed",
          "dmove": "Score"
        },
        {
          "nmove": 64,
          "plid": 22709,
          "movetime": 1649667526091,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302369,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 22709,
            "real_name": "Thierry Pertuy",
            "membership": false,
            "country": "FR"
          },
          "rating": 1756.0692,
          "deviation": 20
        },
        {
          "player": {
            "plid": 8262,
            "real_name": "Zandor",
            "membership": false,
            "country": "AT"
          },
          "rating": 1716.0134,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 0,
      "expire_time": 1650826109376,
      "chngr": [
        -10.2653885,
        10.2653885
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685128,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 22709,
          "movetime": 1648500174897,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 2,
          "plid": 8262,
          "movetime": 1648511121927,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 3,
          "plid": 22709,
          "movetime": 1648539757147,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 4,
          "plid": 8262,
          "movetime": 1648559332702,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 5,
          "plid": 22709,
          "movetime": 1648571255862,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 6,
          "plid": 8262,
          "movetime": 1648665731266,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 7,
          "plid": 22709,
          "movetime": 1648669838020,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 8,
          "plid": 8262,
          "movetime": 1648838623088,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 9,
          "plid": 22709,
          "movetime": 1648938831833,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 10,
          "plid": 8262,
          "movetime": 1649096010242,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 11,
          "plid": 22709,
          "movetime": 1649106298422,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 12,
          "plid": 8262,
          "movetime": 1649108162621,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 13,
          "plid": 22709,
          "movetime": 1649138941714,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 14,
          "plid": 8262,
          "movetime": 1649166378844,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 15,
          "plid": 22709,
          "movetime": 1649173600915,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 16,
          "plid": 8262,
          "movetime": 1649346313666,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 17,
          "plid": 22709,
          "movetime": 1649346872585,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 18,
          "plid": 8262,
          "movetime": 1649348418483,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 19,
          "plid": 22709,
          "movetime": 1649348941524,
          "jmove": "bc",
          "dmove": "B3"
        },
        {
          "nmove": 20,
          "plid": 8262,
          "movetime": 1649443867699,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 21,
          "plid": 22709,
          "movetime": 1649444109376,
          "jmove": "if",
          "dmove": "I6"
        },
        {
          "nmove": 22,
          "plid": 8262,
          "movetime": 1649525811588,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 23,
          "plid": 22709,
          "movetime": 1649526286282,
          "jmove": "ie",
          "dmove": "I5"
        },
        {
          "nmove": 24,
          "plid": 8262,
          "movetime": 1649631117625,
          "jmove": "id",
          "dmove": "I4"
        },
        {
          "nmove": 25,
          "plid": 22709,
          "movetime": 1649662351004,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 26,
          "plid": 8262,
          "movetime": 1649688251562,
          "jmove": "ig",
          "dmove": "I7"
        },
        {
          "nmove": 27,
          "plid": 22709,
          "movetime": 1649704077626,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 28,
          "plid": 8262,
          "movetime": 1649709292798,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 29,
          "plid": 22709,
          "movetime": 1649714995742,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 30,
          "plid": 8262,
          "movetime": 1649723716474,
          "jmove": "ac",
          "dmove": "A3"
        },
        {
          "nmove": 31,
          "plid": 22709,
          "movetime": 1649743641874,
          "jmove": "ab",
          "dmove": "A2"
        },
        {
          "nmove": 32,
          "plid": 8262,
          "movetime": 1649862287303,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 33,
          "plid": 22709,
          "movetime": 1649866482254,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 34,
          "plid": 8262,
          "movetime": 1649937545555,
          "jmove": "bb",
          "dmove": "B2"
        },
        {
          "nmove": 35,
          "plid": 22709,
          "movetime": 1649937739006,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 36,
          "plid": 8262,
          "movetime": 1649948300660,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 37,
          "plid": 22709,
          "movetime": 1649949280885,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 38,
          "plid": 8262,
          "movetime": 1649956348592,
          "jmove": "aa",
          "dmove": "A1"
        },
        {
          "nmove": 39,
          "plid": 22709,
          "movetime": 1649958031954,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 40,
          "plid": 8262,
          "movetime": 1649966384659,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 41,
          "plid": 22709,
          "movetime": 1649975035107,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 42,
          "plid": 8262,
          "movetime": 1650230618528,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 43,
          "plid": 22709,
          "movetime": 1650317190146,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 44,
          "plid": 8262,
          "movetime": 1650367260237,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 45,
          "plid": 22709,
          "movetime": 1650375225719,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 46,
          "plid": 8262,
          "movetime": 1650587664483,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 47,
          "plid": 22709,
          "movetime": 1650608951039,
          "jmove": "ba",
          "dmove": "B1"
        },
        {
          "nmove": 48,
          "plid": 8262,
          "movetime": 1650805387798,
          "jmove": "ab",
          "dmove": "A2"
        },
        {
          "nmove": 49,
          "plid": 22709,
          "movetime": 1650811926949,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 50,
          "plid": 8262,
          "movetime": 1650812119272,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 51,
          "plid": 22709,
          "movetime": 1650815426388,
          "jmove": "scoreid",
          "dmove": "Score"
        },
        {
          "nmove": 52,
          "plid": 8262,
          "movetime": 1650826109368,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        806400000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302370,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 44616,
            "real_name": "nullptr",
            "membership": false,
            "country": "US"
          },
          "rating": 1737.2621,
          "deviation": 20
        },
        {
          "player": {
            "plid": 22709,
            "real_name": "Thierry Pertuy",
            "membership": false,
            "country": "FR"
          },
          "rating": 1756.0692,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 22709,
      "expire_time": 1649081844173,
      "chngr": [
        11.986838,
        -11.986838
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685130,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 44616,
          "movetime": 1648516045526,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 2,
          "plid": 22709,
          "movetime": 1648539805727,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 3,
          "plid": 44616,
          "movetime": 1648603540980,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 4,
          "plid": 22709,
          "movetime": 1648629386039,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 5,
          "plid": 44616,
          "movetime": 1648690264020,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 6,
          "plid": 22709,
          "movetime": 1648744315105,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 7,
          "plid": 44616,
          "movetime": 1648775791829,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 8,
          "plid": 22709,
          "movetime": 1648938596314,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 9,
          "plid": 44616,
          "movetime": 1648951931622,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 10,
          "plid": 22709,
          "movetime": 1648968993131,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 11,
          "plid": 44616,
          "movetime": 1648997032666,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 12,
          "plid": 22709,
          "movetime": 1649010181596,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 13,
          "plid": 44616,
          "movetime": 1649012129177,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 14,
          "plid": 22709,
          "movetime": 1649017690955,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 15,
          "plid": 44616,
          "movetime": 1649019797321,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 16,
          "plid": 22709,
          "movetime": 1649053840102,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 17,
          "plid": 44616,
          "movetime": 1649077056307,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 18,
          "plid": 22709,
          "movetime": 1649081844166,
          "jmove": "resign",
          "dmove": "resign"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302371,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 22709,
            "real_name": "Thierry Pertuy",
            "membership": false,
            "country": "FR"
          },
          "rating": 1756.0692,
          "deviation": 20
        },
        {
          "player": {
            "plid": 4090,
            "real_name": "David Milne",
            "membership": true,
            "country": "NZ"
          },
          "rating": 1551.7124,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 0,
      "expire_time": 1650608973190,
      "chngr": [
        7.8130107,
        -7.8130107
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685133,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 22709,
          "movetime": 1648500183413,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 2,
          "plid": 4090,
          "movetime": 1648512310966,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 3,
          "plid": 22709,
          "movetime": 1648539785078,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 4,
          "plid": 4090,
          "movetime": 1648548301805,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 5,
          "plid": 22709,
          "movetime": 1648565024296,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 6,
          "plid": 4090,
          "movetime": 1648600808034,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 7,
          "plid": 22709,
          "movetime": 1648626099949,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 8,
          "plid": 4090,
          "movetime": 1648639766316,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 9,
          "plid": 22709,
          "movetime": 1648641994395,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 10,
          "plid": 4090,
          "movetime": 1648689304362,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 11,
          "plid": 22709,
          "movetime": 1648727330204,
          "jmove": "if",
          "dmove": "I6"
        },
        {
          "nmove": 12,
          "plid": 4090,
          "movetime": 1648802656751,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 13,
          "plid": 22709,
          "movetime": 1648938710750,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 14,
          "plid": 4090,
          "movetime": 1648960119065,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 15,
          "plid": 22709,
          "movetime": 1648969060503,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 16,
          "plid": 4090,
          "movetime": 1648972990998,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 17,
          "plid": 22709,
          "movetime": 1649010381299,
          "jmove": "bc",
          "dmove": "B3"
        },
        {
          "nmove": 18,
          "plid": 4090,
          "movetime": 1649061759320,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 19,
          "plid": 22709,
          "movetime": 1649063452470,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 20,
          "plid": 4090,
          "movetime": 1649120930101,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 21,
          "plid": 22709,
          "movetime": 1649139019835,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 22,
          "plid": 4090,
          "movetime": 1649208991599,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 23,
          "plid": 22709,
          "movetime": 1649227565353,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 24,
          "plid": 4090,
          "movetime": 1649290797339,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 25,
          "plid": 22709,
          "movetime": 1649316901449,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 26,
          "plid": 4090,
          "movetime": 1649378514110,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 27,
          "plid": 22709,
          "movetime": 1649387522543,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 28,
          "plid": 4090,
          "movetime": 1649469160413,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 29,
          "plid": 22709,
          "movetime": 1649487442368,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 30,
          "plid": 4090,
          "movetime": 1649552830786,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 31,
          "plid": 22709,
          "movetime": 1649568105257,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 32,
          "plid": 4090,
          "movetime": 1649643853965,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 33,
          "plid": 22709,
          "movetime": 1649662386984,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 34,
          "plid": 4090,
          "movetime": 1649727977892,
          "jmove": "bb",
          "dmove": "B2"
        },
        {
          "nmove": 35,
          "plid": 22709,
          "movetime": 1649743773507,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 36,
          "plid": 4090,
          "movetime": 1649815870480,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 37,
          "plid": 22709,
          "movetime": 1649831445711,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 38,
          "plid": 4090,
          "movetime": 1650081569425,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 39,
          "plid": 22709,
          "movetime": 1650097359223,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 40,
          "plid": 4090,
          "movetime": 1650109434332,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 41,
          "plid": 22709,
          "movetime": 1650146966046,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 42,
          "plid": 4090,
          "movetime": 1650157872374,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 43,
          "plid": 22709,
          "movetime": 1650180644554,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 44,
          "plid": 4090,
          "movetime": 1650251456488,
          "jmove": "ih",
          "dmove": "I8"
        },
        {
          "nmove": 45,
          "plid": 22709,
          "movetime": 1650266718793,
          "jmove": "ig",
          "dmove": "I7"
        },
        {
          "nmove": 46,
          "plid": 4090,
          "movetime": 1650324607137,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 47,
          "plid": 22709,
          "movetime": 1650351335293,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 48,
          "plid": 4090,
          "movetime": 1650458183526,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 49,
          "plid": 22709,
          "movetime": 1650458473204,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 50,
          "plid": 4090,
          "movetime": 1650458566837,
          "jmove": "ae",
          "dmove": "A5"
        },
        {
          "nmove": 51,
          "plid": 22709,
          "movetime": 1650468628590,
          "jmove": "ac",
          "dmove": "A3"
        },
        {
          "nmove": 52,
          "plid": 4090,
          "movetime": 1650515229811,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 53,
          "plid": 22709,
          "movetime": 1650523777997,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 54,
          "plid": 4090,
          "movetime": 1650593804943,
          "jmove": "scoreefhc",
          "dmove": "Score"
        },
        {
          "nmove": 55,
          "plid": 22709,
          "movetime": 1650608973185,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302372,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 152553,
            "real_name": "pacmaniac",
            "membership": false,
            "country": "EU"
          },
          "rating": 1825.2876,
          "deviation": 31
        },
        {
          "player": {
            "plid": 22709,
            "real_name": "Thierry Pertuy",
            "membership": false,
            "country": "FR"
          },
          "rating": 1756.0692,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 22709,
      "expire_time": 1650409327697,
      "chngr": [
        48.92765,
        -12.545551
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685135,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 152553,
          "movetime": 1648469084444,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 2,
          "plid": 22709,
          "movetime": 1648500292074,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 3,
          "plid": 152553,
          "movetime": 1648554909039,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 4,
          "plid": 22709,
          "movetime": 1648571177316,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 5,
          "plid": 152553,
          "movetime": 1648649835110,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 6,
          "plid": 22709,
          "movetime": 1648650256184,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 7,
          "plid": 152553,
          "movetime": 1648654127558,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 8,
          "plid": 22709,
          "movetime": 1648669942946,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 9,
          "plid": 152553,
          "movetime": 1648742337206,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 10,
          "plid": 22709,
          "movetime": 1648744363618,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 11,
          "plid": 152553,
          "movetime": 1648817775258,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 12,
          "plid": 22709,
          "movetime": 1648938751491,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 13,
          "plid": 152553,
          "movetime": 1649011534089,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 14,
          "plid": 22709,
          "movetime": 1649014426626,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 15,
          "plid": 152553,
          "movetime": 1649098752231,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 16,
          "plid": 22709,
          "movetime": 1649139131902,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 17,
          "plid": 152553,
          "movetime": 1649186122475,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 18,
          "plid": 22709,
          "movetime": 1649189303919,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 19,
          "plid": 152553,
          "movetime": 1649270677304,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 20,
          "plid": 22709,
          "movetime": 1649278468558,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 21,
          "plid": 152553,
          "movetime": 1649355382168,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 22,
          "plid": 22709,
          "movetime": 1649358481083,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 23,
          "plid": 152553,
          "movetime": 1649510213374,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 24,
          "plid": 22709,
          "movetime": 1649510378234,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 25,
          "plid": 152553,
          "movetime": 1649510398729,
          "jmove": "bh",
          "dmove": "B8"
        },
        {
          "nmove": 26,
          "plid": 22709,
          "movetime": 1649510702433,
          "jmove": "af",
          "dmove": "A6"
        },
        {
          "nmove": 27,
          "plid": 152553,
          "movetime": 1649512167169,
          "jmove": "bb",
          "dmove": "B2"
        },
        {
          "nmove": 28,
          "plid": 22709,
          "movetime": 1649512620320,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 29,
          "plid": 152553,
          "movetime": 1649584836433,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 30,
          "plid": 22709,
          "movetime": 1649587741556,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 31,
          "plid": 152553,
          "movetime": 1649788254820,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 32,
          "plid": 22709,
          "movetime": 1649789570146,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 33,
          "plid": 152553,
          "movetime": 1649790014408,
          "jmove": "ah",
          "dmove": "A8"
        },
        {
          "nmove": 34,
          "plid": 22709,
          "movetime": 1649796957509,
          "jmove": "ag",
          "dmove": "A7"
        },
        {
          "nmove": 35,
          "plid": 152553,
          "movetime": 1649961076269,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 36,
          "plid": 22709,
          "movetime": 1649961209137,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 37,
          "plid": 152553,
          "movetime": 1649961271938,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 38,
          "plid": 22709,
          "movetime": 1649962242873,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 39,
          "plid": 152553,
          "movetime": 1649962866058,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 40,
          "plid": 22709,
          "movetime": 1649963482134,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 41,
          "plid": 152553,
          "movetime": 1650042102827,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 42,
          "plid": 22709,
          "movetime": 1650064649638,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 43,
          "plid": 152553,
          "movetime": 1650117118034,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 44,
          "plid": 22709,
          "movetime": 1650180890215,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 45,
          "plid": 152553,
          "movetime": 1650218144169,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 46,
          "plid": 22709,
          "movetime": 1650234859436,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 47,
          "plid": 152553,
          "movetime": 1650277569355,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 48,
          "plid": 22709,
          "movetime": 1650279858195,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 49,
          "plid": 152553,
          "movetime": 1650306970234,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 50,
          "plid": 22709,
          "movetime": 1650309776570,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 51,
          "plid": 152553,
          "movetime": 1650391542270,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 52,
          "plid": 22709,
          "movetime": 1650409327670,
          "jmove": "resign",
          "dmove": "resign"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302373,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 22709,
            "real_name": "Thierry Pertuy",
            "membership": false,
            "country": "FR"
          },
          "rating": 1756.0692,
          "deviation": 20
        },
        {
          "player": {
            "plid": 144760,
            "real_name": "galispiar",
            "membership": false,
            "country": "JP"
          },
          "rating": 1021.5246,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 144760,
      "expire_time": 1649749682292,
      "chngr": [
        4.252275,
        -12.54421
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685137,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 22709,
          "movetime": 1648500190810,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 2,
          "plid": 144760,
          "movetime": 1649329997210,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 3,
          "plid": 22709,
          "movetime": 1649335236761,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 4,
          "plid": 144760,
          "movetime": 1649401360365,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 5,
          "plid": 22709,
          "movetime": 1649423837313,
          "jmove": "ed",
          "dmove": "E4"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        230400000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302374,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 8262,
            "real_name": "Zandor",
            "membership": false,
            "country": "AT"
          },
          "rating": 1716.0134,
          "deviation": 20
        },
        {
          "player": {
            "plid": 1017,
            "real_name": "Elisa Kabiljo",
            "membership": false,
            "country": "RS"
          },
          "rating": 1698.1548,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 1017,
      "expire_time": 1649968287397,
      "chngr": [
        9.611235,
        -9.611235
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685139,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 8262,
          "movetime": 1648478782385,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 2,
          "plid": 1017,
          "movetime": 1648487211385,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 3,
          "plid": 8262,
          "movetime": 1648511114965,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 4,
          "plid": 1017,
          "movetime": 1648534606141,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 5,
          "plid": 8262,
          "movetime": 1648559329271,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 6,
          "plid": 1017,
          "movetime": 1648576050244,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 7,
          "plid": 8262,
          "movetime": 1648665919140,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 8,
          "plid": 1017,
          "movetime": 1648679596261,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 9,
          "plid": 8262,
          "movetime": 1648838626012,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 10,
          "plid": 1017,
          "movetime": 1648839421806,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 11,
          "plid": 8262,
          "movetime": 1648839493653,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 12,
          "plid": 1017,
          "movetime": 1648839551982,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 13,
          "plid": 8262,
          "movetime": 1648840665345,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 14,
          "plid": 1017,
          "movetime": 1648917463160,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 15,
          "plid": 8262,
          "movetime": 1648922727178,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 16,
          "plid": 1017,
          "movetime": 1648964176030,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 17,
          "plid": 8262,
          "movetime": 1649096039648,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 18,
          "plid": 1017,
          "movetime": 1649097446216,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 19,
          "plid": 8262,
          "movetime": 1649108181127,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 20,
          "plid": 1017,
          "movetime": 1649532464986,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 21,
          "plid": 8262,
          "movetime": 1649631130194,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 22,
          "plid": 1017,
          "movetime": 1649829088518,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 23,
          "plid": 8262,
          "movetime": 1649862308867,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 24,
          "plid": 1017,
          "movetime": 1649862940093,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 25,
          "plid": 8262,
          "movetime": 1649865035148,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 26,
          "plid": 1017,
          "movetime": 1649968287384,
          "jmove": "resign",
          "dmove": "resign"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        637200000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302375,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 1017,
            "real_name": "Elisa Kabiljo",
            "membership": false,
            "country": "RS"
          },
          "rating": 1698.1548,
          "deviation": 20
        },
        {
          "player": {
            "plid": 44616,
            "real_name": "nullptr",
            "membership": false,
            "country": "US"
          },
          "rating": 1737.2621,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 0,
      "expire_time": 1650173238820,
      "chngr": [
        -10.22048,
        10.22048
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685141,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 1017,
          "movetime": 1648457775873,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 2,
          "plid": 44616,
          "movetime": 1648516089603,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 3,
          "plid": 1017,
          "movetime": 1648534624398,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 4,
          "plid": 44616,
          "movetime": 1648603530683,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 5,
          "plid": 1017,
          "movetime": 1648618972760,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 6,
          "plid": 44616,
          "movetime": 1648628172884,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 7,
          "plid": 1017,
          "movetime": 1648659178212,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 8,
          "plid": 44616,
          "movetime": 1648690414524,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 9,
          "plid": 1017,
          "movetime": 1648717292419,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 10,
          "plid": 44616,
          "movetime": 1648729889566,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 11,
          "plid": 1017,
          "movetime": 1648754572344,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 12,
          "plid": 44616,
          "movetime": 1648775803160,
          "jmove": "bc",
          "dmove": "B3"
        },
        {
          "nmove": 13,
          "plid": 1017,
          "movetime": 1648793083042,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 14,
          "plid": 44616,
          "movetime": 1648856754336,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 15,
          "plid": 1017,
          "movetime": 1648879149731,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 16,
          "plid": 44616,
          "movetime": 1648951855690,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 17,
          "plid": 1017,
          "movetime": 1648964211062,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 18,
          "plid": 44616,
          "movetime": 1648996992166,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 19,
          "plid": 1017,
          "movetime": 1649002483903,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 20,
          "plid": 44616,
          "movetime": 1649012122639,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 21,
          "plid": 1017,
          "movetime": 1649024656035,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 22,
          "plid": 44616,
          "movetime": 1649037551529,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 23,
          "plid": 1017,
          "movetime": 1649054048335,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 24,
          "plid": 44616,
          "movetime": 1649077094088,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 25,
          "plid": 1017,
          "movetime": 1649097440067,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 26,
          "plid": 44616,
          "movetime": 1649129461008,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 27,
          "plid": 1017,
          "movetime": 1649135098187,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 28,
          "plid": 44616,
          "movetime": 1649206939796,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 29,
          "plid": 1017,
          "movetime": 1649224991815,
          "jmove": "fa",
          "dmove": "F1"
        },
        {
          "nmove": 30,
          "plid": 44616,
          "movetime": 1649294065986,
          "jmove": "if",
          "dmove": "I6"
        },
        {
          "nmove": 31,
          "plid": 1017,
          "movetime": 1649331940776,
          "jmove": "ie",
          "dmove": "I5"
        },
        {
          "nmove": 32,
          "plid": 44616,
          "movetime": 1649359910090,
          "jmove": "ig",
          "dmove": "I7"
        },
        {
          "nmove": 33,
          "plid": 1017,
          "movetime": 1649367802964,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 34,
          "plid": 44616,
          "movetime": 1649375415870,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 35,
          "plid": 1017,
          "movetime": 1649453289383,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 36,
          "plid": 44616,
          "movetime": 1649562718133,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 37,
          "plid": 1017,
          "movetime": 1649567890620,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 38,
          "plid": 44616,
          "movetime": 1649638546998,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 39,
          "plid": 1017,
          "movetime": 1649659437360,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 40,
          "plid": 44616,
          "movetime": 1649724263200,
          "jmove": "ea",
          "dmove": "E1"
        },
        {
          "nmove": 41,
          "plid": 1017,
          "movetime": 1649742401092,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 42,
          "plid": 44616,
          "movetime": 1649768630835,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 43,
          "plid": 1017,
          "movetime": 1649800958271,
          "jmove": "ah",
          "dmove": "A8"
        },
        {
          "nmove": 44,
          "plid": 44616,
          "movetime": 1649895675277,
          "jmove": "ae",
          "dmove": "A5"
        },
        {
          "nmove": 45,
          "plid": 1017,
          "movetime": 1649917463229,
          "jmove": "af",
          "dmove": "A6"
        },
        {
          "nmove": 46,
          "plid": 44616,
          "movetime": 1649979985645,
          "jmove": "ac",
          "dmove": "A3"
        },
        {
          "nmove": 47,
          "plid": 1017,
          "movetime": 1649999718970,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 48,
          "plid": 44616,
          "movetime": 1650008068710,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 49,
          "plid": 1017,
          "movetime": 1650040455742,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 50,
          "plid": 44616,
          "movetime": 1650061094039,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 51,
          "plid": 1017,
          "movetime": 1650088536163,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 52,
          "plid": 44616,
          "movetime": 1650153982532,
          "jmove": "score",
          "dmove": "Score"
        },
        {
          "nmove": 53,
          "plid": 1017,
          "movetime": 1650173238815,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302376,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 4090,
            "real_name": "David Milne",
            "membership": true,
            "country": "NZ"
          },
          "rating": 1551.7124,
          "deviation": 20
        },
        {
          "player": {
            "plid": 1017,
            "real_name": "Elisa Kabiljo",
            "membership": false,
            "country": "RS"
          },
          "rating": 1698.1548,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 1017,
      "expire_time": 1649800934540,
      "chngr": [
        12.459313,
        -12.459313
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685143,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 4090,
          "movetime": 1648456019613,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 2,
          "plid": 1017,
          "movetime": 1648457801464,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 3,
          "plid": 4090,
          "movetime": 1648457856031,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 4,
          "plid": 1017,
          "movetime": 1648487173001,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 5,
          "plid": 4090,
          "movetime": 1648512185711,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 6,
          "plid": 1017,
          "movetime": 1648534614433,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 7,
          "plid": 4090,
          "movetime": 1648548288011,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 8,
          "plid": 1017,
          "movetime": 1648576026265,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 9,
          "plid": 4090,
          "movetime": 1648600824252,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 10,
          "plid": 1017,
          "movetime": 1648618867957,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 11,
          "plid": 4090,
          "movetime": 1648639757237,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 12,
          "plid": 1017,
          "movetime": 1648659202691,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 13,
          "plid": 4090,
          "movetime": 1648689352708,
          "jmove": "bc",
          "dmove": "B3"
        },
        {
          "nmove": 14,
          "plid": 1017,
          "movetime": 1648717282605,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 15,
          "plid": 4090,
          "movetime": 1648802640856,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 16,
          "plid": 1017,
          "movetime": 1648839453850,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 17,
          "plid": 4090,
          "movetime": 1648862615449,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 18,
          "plid": 1017,
          "movetime": 1648879164769,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 19,
          "plid": 4090,
          "movetime": 1648892907147,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 20,
          "plid": 1017,
          "movetime": 1648908752942,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 21,
          "plid": 4090,
          "movetime": 1648960018931,
          "jmove": "ba",
          "dmove": "B1"
        },
        {
          "nmove": 22,
          "plid": 1017,
          "movetime": 1648964224472,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 23,
          "plid": 4090,
          "movetime": 1648965569970,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 24,
          "plid": 1017,
          "movetime": 1648980353071,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 25,
          "plid": 4090,
          "movetime": 1648988217928,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 26,
          "plid": 1017,
          "movetime": 1649002471474,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 27,
          "plid": 4090,
          "movetime": 1649061683282,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 28,
          "plid": 1017,
          "movetime": 1649097430813,
          "jmove": "if",
          "dmove": "I6"
        },
        {
          "nmove": 29,
          "plid": 4090,
          "movetime": 1649121102881,
          "jmove": "ib",
          "dmove": "I2"
        },
        {
          "nmove": 30,
          "plid": 1017,
          "movetime": 1649135092406,
          "jmove": "ha",
          "dmove": "H1"
        },
        {
          "nmove": 31,
          "plid": 4090,
          "movetime": 1649208926112,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 32,
          "plid": 1017,
          "movetime": 1649279188474,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 33,
          "plid": 4090,
          "movetime": 1649290932019,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 34,
          "plid": 1017,
          "movetime": 1649338654637,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 35,
          "plid": 4090,
          "movetime": 1649378604284,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 36,
          "plid": 1017,
          "movetime": 1649453374064,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 37,
          "plid": 4090,
          "movetime": 1649469262181,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 38,
          "plid": 1017,
          "movetime": 1649479919072,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 39,
          "plid": 4090,
          "movetime": 1649552707211,
          "jmove": "id",
          "dmove": "I4"
        },
        {
          "nmove": 40,
          "plid": 1017,
          "movetime": 1649800934505,
          "jmove": "resign",
          "dmove": "resign"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302377,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 1017,
            "real_name": "Elisa Kabiljo",
            "membership": false,
            "country": "RS"
          },
          "rating": 1698.1548,
          "deviation": 20
        },
        {
          "player": {
            "plid": 152553,
            "real_name": "pacmaniac",
            "membership": false,
            "country": "EU"
          },
          "rating": 1825.2876,
          "deviation": 31
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 0,
      "expire_time": 1651561331195,
      "chngr": [
        -8.528236,
        30.275238
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685145,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 1017,
          "movetime": 1648457787894,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 2,
          "plid": 152553,
          "movetime": 1648469154468,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 3,
          "plid": 1017,
          "movetime": 1648487196046,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 4,
          "plid": 152553,
          "movetime": 1648554876025,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 5,
          "plid": 1017,
          "movetime": 1648576045641,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 6,
          "plid": 152553,
          "movetime": 1648649893277,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 7,
          "plid": 1017,
          "movetime": 1648659159787,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 8,
          "plid": 152553,
          "movetime": 1648742302013,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 9,
          "plid": 1017,
          "movetime": 1648754593182,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 10,
          "plid": 152553,
          "movetime": 1648817831103,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 11,
          "plid": 1017,
          "movetime": 1648834913608,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 12,
          "plid": 152553,
          "movetime": 1648898287633,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 13,
          "plid": 1017,
          "movetime": 1648908766647,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 14,
          "plid": 152553,
          "movetime": 1649011463468,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 15,
          "plid": 1017,
          "movetime": 1649024643079,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 16,
          "plid": 152553,
          "movetime": 1649098813961,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 17,
          "plid": 1017,
          "movetime": 1649104062170,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 18,
          "plid": 152553,
          "movetime": 1649185937100,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 19,
          "plid": 1017,
          "movetime": 1649532529351,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 20,
          "plid": 152553,
          "movetime": 1649584883695,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 21,
          "plid": 1017,
          "movetime": 1649609864630,
          "jmove": "ea",
          "dmove": "E1"
        },
        {
          "nmove": 22,
          "plid": 152553,
          "movetime": 1649788308529,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 23,
          "plid": 1017,
          "movetime": 1649800940605,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 24,
          "plid": 152553,
          "movetime": 1649961036458,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 25,
          "plid": 1017,
          "movetime": 1649968323826,
          "jmove": "fa",
          "dmove": "F1"
        },
        {
          "nmove": 26,
          "plid": 152553,
          "movetime": 1650042065765,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 27,
          "plid": 1017,
          "movetime": 1650219935975,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 28,
          "plid": 152553,
          "movetime": 1650277518318,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 29,
          "plid": 1017,
          "movetime": 1650286842306,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 30,
          "plid": 152553,
          "movetime": 1650307026167,
          "jmove": "bh",
          "dmove": "B8"
        },
        {
          "nmove": 31,
          "plid": 1017,
          "movetime": 1650656828099,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 32,
          "plid": 152553,
          "movetime": 1650739097934,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 33,
          "plid": 1017,
          "movetime": 1651002924970,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 34,
          "plid": 152553,
          "movetime": 1651084923986,
          "jmove": "bi",
          "dmove": "B9"
        },
        {
          "nmove": 35,
          "plid": 1017,
          "movetime": 1651167111307,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 36,
          "plid": 152553,
          "movetime": 1651167839258,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 37,
          "plid": 1017,
          "movetime": 1651180285620,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 38,
          "plid": 152553,
          "movetime": 1651338485929,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 39,
          "plid": 1017,
          "movetime": 1651351011296,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 40,
          "plid": 152553,
          "movetime": 1651385030755,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 41,
          "plid": 1017,
          "movetime": 1651421143456,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 42,
          "plid": 152553,
          "movetime": 1651428787510,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 43,
          "plid": 1017,
          "movetime": 1651436313819,
          "jmove": "scorece",
          "dmove": "Score"
        },
        {
          "nmove": 44,
          "plid": 152553,
          "movetime": 1651561331188,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302378,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 144760,
            "real_name": "galispiar",
            "membership": false,
            "country": "JP"
          },
          "rating": 1021.5246,
          "deviation": 20
        },
        {
          "player": {
            "plid": 1017,
            "real_name": "Elisa Kabiljo",
            "membership": false,
            "country": "RS"
          },
          "rating": 1698.1548,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 144760,
      "expire_time": 1649749683339,
      "chngr": [
        -10.859259,
        3.8783066
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685147,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 144760,
          "movetime": 1649154067726,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 2,
          "plid": 1017,
          "movetime": 1649182072470,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 3,
          "plid": 144760,
          "movetime": 1649401183712,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 4,
          "plid": 1017,
          "movetime": 1649453514375,
          "jmove": "cd",
          "dmove": "C4"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        208800000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302379,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 44616,
            "real_name": "nullptr",
            "membership": false,
            "country": "US"
          },
          "rating": 1737.2621,
          "deviation": 20
        },
        {
          "player": {
            "plid": 8262,
            "real_name": "Zandor",
            "membership": false,
            "country": "AT"
          },
          "rating": 1716.0134,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 0,
      "expire_time": 1651632705177,
      "chngr": [
        -8.396401,
        8.396401
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685149,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 44616,
          "movetime": 1648516052907,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 2,
          "plid": 8262,
          "movetime": 1648559311455,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 3,
          "plid": 44616,
          "movetime": 1648603576308,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 4,
          "plid": 8262,
          "movetime": 1648665926427,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 5,
          "plid": 44616,
          "movetime": 1648690422612,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 6,
          "plid": 8262,
          "movetime": 1648838659466,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 7,
          "plid": 44616,
          "movetime": 1648856924739,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 8,
          "plid": 8262,
          "movetime": 1648922682864,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 9,
          "plid": 44616,
          "movetime": 1648951912049,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 10,
          "plid": 8262,
          "movetime": 1649096023884,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 11,
          "plid": 44616,
          "movetime": 1649129405164,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 12,
          "plid": 8262,
          "movetime": 1649166306440,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 13,
          "plid": 44616,
          "movetime": 1649206960094,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 14,
          "plid": 8262,
          "movetime": 1649346322395,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 15,
          "plid": 44616,
          "movetime": 1649359934225,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 16,
          "plid": 8262,
          "movetime": 1649443877946,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 17,
          "plid": 44616,
          "movetime": 1649562707367,
          "jmove": "bh",
          "dmove": "B8"
        },
        {
          "nmove": 18,
          "plid": 8262,
          "movetime": 1649631140725,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 19,
          "plid": 44616,
          "movetime": 1649638672862,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 20,
          "plid": 8262,
          "movetime": 1649688238116,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 21,
          "plid": 44616,
          "movetime": 1649724303984,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 22,
          "plid": 8262,
          "movetime": 1649862275407,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 23,
          "plid": 44616,
          "movetime": 1649895715504,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 24,
          "plid": 8262,
          "movetime": 1649937590114,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 25,
          "plid": 44616,
          "movetime": 1649979999979,
          "jmove": "ig",
          "dmove": "I7"
        },
        {
          "nmove": 26,
          "plid": 8262,
          "movetime": 1650230628193,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 27,
          "plid": 44616,
          "movetime": 1650331107624,
          "jmove": "gi",
          "dmove": "G9"
        },
        {
          "nmove": 28,
          "plid": 8262,
          "movetime": 1650367264553,
          "jmove": "ah",
          "dmove": "A8"
        },
        {
          "nmove": 29,
          "plid": 44616,
          "movetime": 1650370783947,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 30,
          "plid": 8262,
          "movetime": 1650587671738,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 31,
          "plid": 44616,
          "movetime": 1650631855937,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 32,
          "plid": 8262,
          "movetime": 1650805403605,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 33,
          "plid": 44616,
          "movetime": 1650809866054,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 34,
          "plid": 8262,
          "movetime": 1650812128943,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 35,
          "plid": 44616,
          "movetime": 1650942275892,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 36,
          "plid": 8262,
          "movetime": 1651015171657,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 37,
          "plid": 44616,
          "movetime": 1651106828034,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 38,
          "plid": 8262,
          "movetime": 1651107288570,
          "jmove": "fa",
          "dmove": "F1"
        },
        {
          "nmove": 39,
          "plid": 44616,
          "movetime": 1651107457093,
          "jmove": "ga",
          "dmove": "G1"
        },
        {
          "nmove": 40,
          "plid": 8262,
          "movetime": 1651155421980,
          "jmove": "ea",
          "dmove": "E1"
        },
        {
          "nmove": 41,
          "plid": 44616,
          "movetime": 1651162660238,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 42,
          "plid": 8262,
          "movetime": 1651182305936,
          "jmove": "ag",
          "dmove": "A7"
        },
        {
          "nmove": 43,
          "plid": 44616,
          "movetime": 1651198305097,
          "jmove": "bi",
          "dmove": "B9"
        },
        {
          "nmove": 44,
          "plid": 8262,
          "movetime": 1651239720244,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 45,
          "plid": 44616,
          "movetime": 1651285037105,
          "jmove": "ai",
          "dmove": "A9"
        },
        {
          "nmove": 46,
          "plid": 8262,
          "movetime": 1651320234021,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 47,
          "plid": 44616,
          "movetime": 1651324585882,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 48,
          "plid": 8262,
          "movetime": 1651341702556,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 49,
          "plid": 44616,
          "movetime": 1651364923678,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 50,
          "plid": 8262,
          "movetime": 1651492678451,
          "jmove": "score",
          "dmove": "Score"
        },
        {
          "nmove": 51,
          "plid": 44616,
          "movetime": 1651632705170,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302380,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 8262,
            "real_name": "Zandor",
            "membership": false,
            "country": "AT"
          },
          "rating": 1716.0134,
          "deviation": 20
        },
        {
          "player": {
            "plid": 4090,
            "real_name": "David Milne",
            "membership": true,
            "country": "NZ"
          },
          "rating": 1551.7124,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 0,
      "expire_time": 1652844655948,
      "chngr": [
        6.8646474,
        -6.8646474
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685151,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 8262,
          "movetime": 1648478787352,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 2,
          "plid": 4090,
          "movetime": 1648512166703,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 3,
          "plid": 8262,
          "movetime": 1648514326225,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 4,
          "plid": 4090,
          "movetime": 1648548256068,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 5,
          "plid": 8262,
          "movetime": 1648559335822,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 6,
          "plid": 4090,
          "movetime": 1648600683818,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 7,
          "plid": 8262,
          "movetime": 1648665923871,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 8,
          "plid": 4090,
          "movetime": 1648689359912,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 9,
          "plid": 8262,
          "movetime": 1648838632172,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 10,
          "plid": 4090,
          "movetime": 1648862599617,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 11,
          "plid": 8262,
          "movetime": 1648922693512,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 12,
          "plid": 4090,
          "movetime": 1648960094011,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 13,
          "plid": 8262,
          "movetime": 1649096030888,
          "jmove": "ib",
          "dmove": "I2"
        },
        {
          "nmove": 14,
          "plid": 4090,
          "movetime": 1649121082124,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 15,
          "plid": 8262,
          "movetime": 1649166362565,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 16,
          "plid": 4090,
          "movetime": 1649209065431,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 17,
          "plid": 8262,
          "movetime": 1649346333752,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 18,
          "plid": 4090,
          "movetime": 1649378637107,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 19,
          "plid": 8262,
          "movetime": 1649443893767,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 20,
          "plid": 4090,
          "movetime": 1649469244036,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 21,
          "plid": 8262,
          "movetime": 1649525820932,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 22,
          "plid": 4090,
          "movetime": 1649552948027,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 23,
          "plid": 8262,
          "movetime": 1649631135660,
          "jmove": "fa",
          "dmove": "F1"
        },
        {
          "nmove": 24,
          "plid": 4090,
          "movetime": 1649644702394,
          "jmove": "bc",
          "dmove": "B3"
        },
        {
          "nmove": 25,
          "plid": 8262,
          "movetime": 1649688242060,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 26,
          "plid": 4090,
          "movetime": 1649728059557,
          "jmove": "bb",
          "dmove": "B2"
        },
        {
          "nmove": 27,
          "plid": 8262,
          "movetime": 1649862280991,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 28,
          "plid": 4090,
          "movetime": 1650082265203,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 29,
          "plid": 8262,
          "movetime": 1650230659302,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 30,
          "plid": 4090,
          "movetime": 1650251627060,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 31,
          "plid": 8262,
          "movetime": 1650367282448,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 32,
          "plid": 4090,
          "movetime": 1650458211205,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 33,
          "plid": 8262,
          "movetime": 1650587686265,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 34,
          "plid": 4090,
          "movetime": 1650593935594,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 35,
          "plid": 8262,
          "movetime": 1650805418120,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 36,
          "plid": 4090,
          "movetime": 1650857922256,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 37,
          "plid": 8262,
          "movetime": 1650891540552,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 38,
          "plid": 4090,
          "movetime": 1650892868174,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 39,
          "plid": 8262,
          "movetime": 1651015143256,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 40,
          "plid": 4090,
          "movetime": 1651023651362,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 41,
          "plid": 8262,
          "movetime": 1651107252170,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 42,
          "plid": 4090,
          "movetime": 1651125858852,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 43,
          "plid": 8262,
          "movetime": 1651155449688,
          "jmove": "bh",
          "dmove": "B8"
        },
        {
          "nmove": 44,
          "plid": 4090,
          "movetime": 1651201438207,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 45,
          "plid": 8262,
          "movetime": 1651239723257,
          "jmove": "ag",
          "dmove": "A7"
        },
        {
          "nmove": 46,
          "plid": 4090,
          "movetime": 1651288995526,
          "jmove": "ba",
          "dmove": "B1"
        },
        {
          "nmove": 47,
          "plid": 8262,
          "movetime": 1651320257094,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 48,
          "plid": 4090,
          "movetime": 1651375135027,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 49,
          "plid": 8262,
          "movetime": 1651492775853,
          "jmove": "ah",
          "dmove": "A8"
        },
        {
          "nmove": 50,
          "plid": 4090,
          "movetime": 1651545183449,
          "jmove": "bi",
          "dmove": "B9"
        },
        {
          "nmove": 51,
          "plid": 8262,
          "movetime": 1651576078942,
          "jmove": "ai",
          "dmove": "A9"
        },
        {
          "nmove": 52,
          "plid": 4090,
          "movetime": 1651576750025,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 53,
          "plid": 8262,
          "movetime": 1651686064793,
          "jmove": "af",
          "dmove": "A6"
        },
        {
          "nmove": 54,
          "plid": 4090,
          "movetime": 1651721084326,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 55,
          "plid": 8262,
          "movetime": 1651755071886,
          "jmove": "ab",
          "dmove": "A2"
        },
        {
          "nmove": 56,
          "plid": 4090,
          "movetime": 1651834669961,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 57,
          "plid": 8262,
          "movetime": 1651921243273,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 58,
          "plid": 4090,
          "movetime": 1651923567970,
          "jmove": "bi",
          "dmove": "B9"
        },
        {
          "nmove": 59,
          "plid": 8262,
          "movetime": 1651927042078,
          "jmove": "fi",
          "dmove": "F9"
        },
        {
          "nmove": 60,
          "plid": 4090,
          "movetime": 1651981610046,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 61,
          "plid": 8262,
          "movetime": 1652043145287,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 62,
          "plid": 4090,
          "movetime": 1652058589961,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 63,
          "plid": 8262,
          "movetime": 1652270028855,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 64,
          "plid": 4090,
          "movetime": 1652270098768,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 65,
          "plid": 8262,
          "movetime": 1652270696964,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 66,
          "plid": 4090,
          "movetime": 1652322513412,
          "jmove": "bi",
          "dmove": "B9"
        },
        {
          "nmove": 67,
          "plid": 8262,
          "movetime": 1652345540971,
          "jmove": "ie",
          "dmove": "I5"
        },
        {
          "nmove": 68,
          "plid": 4090,
          "movetime": 1652353496458,
          "jmove": "gi",
          "dmove": "G9"
        },
        {
          "nmove": 69,
          "plid": 8262,
          "movetime": 1652401480273,
          "jmove": "if",
          "dmove": "I6"
        },
        {
          "nmove": 70,
          "plid": 4090,
          "movetime": 1652410584144,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 71,
          "plid": 8262,
          "movetime": 1652462575642,
          "jmove": "ih",
          "dmove": "I8"
        },
        {
          "nmove": 72,
          "plid": 4090,
          "movetime": 1652486374064,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 73,
          "plid": 8262,
          "movetime": 1652575536498,
          "jmove": "ig",
          "dmove": "I7"
        },
        {
          "nmove": 74,
          "plid": 4090,
          "movetime": 1652580536198,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 75,
          "plid": 8262,
          "movetime": 1652721023651,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 76,
          "plid": 4090,
          "movetime": 1652755952236,
          "jmove": "scorebahb",
          "dmove": "Score"
        },
        {
          "nmove": 77,
          "plid": 8262,
          "movetime": 1652811738730,
          "jmove": "scorecdhbdh",
          "dmove": "Score"
        },
        {
          "nmove": 78,
          "plid": 4090,
          "movetime": 1652844655940,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302381,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 152553,
            "real_name": "pacmaniac",
            "membership": false,
            "country": "EU"
          },
          "rating": 1825.2876,
          "deviation": 31
        },
        {
          "player": {
            "plid": 8262,
            "real_name": "Zandor",
            "membership": false,
            "country": "AT"
          },
          "rating": 1716.0134,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 0,
      "expire_time": 1651167766901,
      "chngr": [
        37.391796,
        -10.38661
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685153,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 152553,
          "movetime": 1648469103800,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 2,
          "plid": 8262,
          "movetime": 1648478795081,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 3,
          "plid": 152553,
          "movetime": 1648554821289,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 4,
          "plid": 8262,
          "movetime": 1648559340161,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 5,
          "plid": 152553,
          "movetime": 1648649796616,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 6,
          "plid": 8262,
          "movetime": 1648665929263,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 7,
          "plid": 152553,
          "movetime": 1648742317780,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 8,
          "plid": 8262,
          "movetime": 1648838752658,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 9,
          "plid": 152553,
          "movetime": 1648898318999,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 10,
          "plid": 8262,
          "movetime": 1648922713648,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 11,
          "plid": 152553,
          "movetime": 1649011489000,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 12,
          "plid": 8262,
          "movetime": 1649096054851,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 13,
          "plid": 152553,
          "movetime": 1649098914646,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 14,
          "plid": 8262,
          "movetime": 1649108204057,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 15,
          "plid": 152553,
          "movetime": 1649185959645,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 16,
          "plid": 8262,
          "movetime": 1649346319077,
          "jmove": "ic",
          "dmove": "I3"
        },
        {
          "nmove": 17,
          "plid": 152553,
          "movetime": 1649355714042,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 18,
          "plid": 8262,
          "movetime": 1649443861580,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 19,
          "plid": 152553,
          "movetime": 1649510358547,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 20,
          "plid": 8262,
          "movetime": 1649525831749,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 21,
          "plid": 152553,
          "movetime": 1649584861723,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 22,
          "plid": 8262,
          "movetime": 1649631156841,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 23,
          "plid": 152553,
          "movetime": 1649788365924,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 24,
          "plid": 8262,
          "movetime": 1649862304934,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 25,
          "plid": 152553,
          "movetime": 1649961136486,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 26,
          "plid": 8262,
          "movetime": 1649966392558,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 27,
          "plid": 152553,
          "movetime": 1650042120603,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 28,
          "plid": 8262,
          "movetime": 1650230650618,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 29,
          "plid": 152553,
          "movetime": 1650277552262,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 30,
          "plid": 8262,
          "movetime": 1650367275198,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 31,
          "plid": 152553,
          "movetime": 1650391660944,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 32,
          "plid": 8262,
          "movetime": 1650587678267,
          "jmove": "ae",
          "dmove": "A5"
        },
        {
          "nmove": 33,
          "plid": 152553,
          "movetime": 1650738965246,
          "jmove": "af",
          "dmove": "A6"
        },
        {
          "nmove": 34,
          "plid": 8262,
          "movetime": 1650805421519,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 35,
          "plid": 152553,
          "movetime": 1650824919486,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 36,
          "plid": 8262,
          "movetime": 1650826124014,
          "jmove": "ie",
          "dmove": "I5"
        },
        {
          "nmove": 37,
          "plid": 152553,
          "movetime": 1650826247118,
          "jmove": "if",
          "dmove": "I6"
        },
        {
          "nmove": 38,
          "plid": 8262,
          "movetime": 1650891552373,
          "jmove": "id",
          "dmove": "I4"
        },
        {
          "nmove": 39,
          "plid": 152553,
          "movetime": 1650908977857,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 40,
          "plid": 8262,
          "movetime": 1651015160655,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 41,
          "plid": 152553,
          "movetime": 1651084967650,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 42,
          "plid": 8262,
          "movetime": 1651107276212,
          "jmove": "scoregf",
          "dmove": "Score"
        },
        {
          "nmove": 43,
          "plid": 152553,
          "movetime": 1651167766895,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302382,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 8262,
            "real_name": "Zandor",
            "membership": false,
            "country": "AT"
          },
          "rating": 1716.0134,
          "deviation": 20
        },
        {
          "player": {
            "plid": 144760,
            "real_name": "galispiar",
            "membership": false,
            "country": "JP"
          },
          "rating": 1021.5246,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 144760,
      "expire_time": 1649749682574,
      "chngr": [
        4.72626,
        -13.706155
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685155,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 8262,
          "movetime": 1648478791646,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 2,
          "plid": 144760,
          "movetime": 1649154239148,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 3,
          "plid": 8262,
          "movetime": 1649166381950,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 4,
          "plid": 144760,
          "movetime": 1649401290255,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 5,
          "plid": 8262,
          "movetime": 1649443896147,
          "jmove": "db",
          "dmove": "D2"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        216000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302383,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 4090,
            "real_name": "David Milne",
            "membership": true,
            "country": "NZ"
          },
          "rating": 1551.7124,
          "deviation": 20
        },
        {
          "player": {
            "plid": 44616,
            "real_name": "nullptr",
            "membership": false,
            "country": "US"
          },
          "rating": 1737.2621,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 44616,
      "expire_time": 1650977151794,
      "chngr": [
        11.216886,
        -11.216886
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685157,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 4090,
          "movetime": 1648456032182,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 2,
          "plid": 44616,
          "movetime": 1648516077294,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 3,
          "plid": 4090,
          "movetime": 1648548262752,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 4,
          "plid": 44616,
          "movetime": 1648603551983,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 5,
          "plid": 4090,
          "movetime": 1648639656855,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 6,
          "plid": 44616,
          "movetime": 1648690337741,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 7,
          "plid": 4090,
          "movetime": 1648802610043,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 8,
          "plid": 44616,
          "movetime": 1648856849255,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 9,
          "plid": 4090,
          "movetime": 1648862685511,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 10,
          "plid": 44616,
          "movetime": 1648951814382,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 11,
          "plid": 4090,
          "movetime": 1648960129517,
          "jmove": "bb",
          "dmove": "B2"
        },
        {
          "nmove": 12,
          "plid": 44616,
          "movetime": 1648996977298,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 13,
          "plid": 4090,
          "movetime": 1649061574560,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 14,
          "plid": 44616,
          "movetime": 1649077110131,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 15,
          "plid": 4090,
          "movetime": 1649120979945,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 16,
          "plid": 44616,
          "movetime": 1649129511529,
          "jmove": "fa",
          "dmove": "F1"
        },
        {
          "nmove": 17,
          "plid": 4090,
          "movetime": 1649208869408,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 18,
          "plid": 44616,
          "movetime": 1649212259612,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 19,
          "plid": 4090,
          "movetime": 1649290736433,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 20,
          "plid": 44616,
          "movetime": 1649294189972,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 21,
          "plid": 4090,
          "movetime": 1649378399673,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 22,
          "plid": 44616,
          "movetime": 1649384495039,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 23,
          "plid": 4090,
          "movetime": 1649469125023,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 24,
          "plid": 44616,
          "movetime": 1649562761911,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 25,
          "plid": 4090,
          "movetime": 1649643807595,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 26,
          "plid": 44616,
          "movetime": 1649724217445,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 27,
          "plid": 4090,
          "movetime": 1649728101793,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 28,
          "plid": 44616,
          "movetime": 1649731838632,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 29,
          "plid": 4090,
          "movetime": 1649815778218,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 30,
          "plid": 44616,
          "movetime": 1649895689973,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 31,
          "plid": 4090,
          "movetime": 1650082317851,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 32,
          "plid": 44616,
          "movetime": 1650153860539,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 33,
          "plid": 4090,
          "movetime": 1650157977880,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 34,
          "plid": 44616,
          "movetime": 1650330993649,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 35,
          "plid": 4090,
          "movetime": 1650458105718,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 36,
          "plid": 44616,
          "movetime": 1650501431257,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 37,
          "plid": 4090,
          "movetime": 1650515384242,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 38,
          "plid": 44616,
          "movetime": 1650544589733,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 39,
          "plid": 4090,
          "movetime": 1650593842159,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 40,
          "plid": 44616,
          "movetime": 1650631908333,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 41,
          "plid": 4090,
          "movetime": 1650677163484,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 42,
          "plid": 44616,
          "movetime": 1650689031675,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 43,
          "plid": 4090,
          "movetime": 1650718486732,
          "jmove": "ga",
          "dmove": "G1"
        },
        {
          "nmove": 44,
          "plid": 44616,
          "movetime": 1650728530840,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 45,
          "plid": 4090,
          "movetime": 1650766536076,
          "jmove": "ba",
          "dmove": "B1"
        },
        {
          "nmove": 46,
          "plid": 44616,
          "movetime": 1650809740380,
          "jmove": "bc",
          "dmove": "B3"
        },
        {
          "nmove": 47,
          "plid": 4090,
          "movetime": 1650857939857,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 48,
          "plid": 44616,
          "movetime": 1650942371957,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 49,
          "plid": 4090,
          "movetime": 1650945378376,
          "jmove": "ac",
          "dmove": "A3"
        },
        {
          "nmove": 50,
          "plid": 44616,
          "movetime": 1650977151786,
          "jmove": "resign",
          "dmove": "resign"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302384,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 44616,
            "real_name": "nullptr",
            "membership": false,
            "country": "US"
          },
          "rating": 1737.2621,
          "deviation": 20
        },
        {
          "player": {
            "plid": 152553,
            "real_name": "pacmaniac",
            "membership": false,
            "country": "EU"
          },
          "rating": 1825.2876,
          "deviation": 31
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 0,
      "expire_time": 1650995238951,
      "chngr": [
        -9.641316,
        35.190804
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685159,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 44616,
          "movetime": 1648516067513,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 2,
          "plid": 152553,
          "movetime": 1648554996680,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 3,
          "plid": 44616,
          "movetime": 1648603562996,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 4,
          "plid": 152553,
          "movetime": 1648649953447,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 5,
          "plid": 44616,
          "movetime": 1648690391009,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 6,
          "plid": 152553,
          "movetime": 1648742434073,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 7,
          "plid": 44616,
          "movetime": 1648775779235,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 8,
          "plid": 152553,
          "movetime": 1648817888971,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 9,
          "plid": 44616,
          "movetime": 1648856906799,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 10,
          "plid": 152553,
          "movetime": 1648898343151,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 11,
          "plid": 44616,
          "movetime": 1648951885904,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 12,
          "plid": 152553,
          "movetime": 1649011558533,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 13,
          "plid": 44616,
          "movetime": 1649012141355,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 14,
          "plid": 152553,
          "movetime": 1649013571646,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 15,
          "plid": 44616,
          "movetime": 1649019760116,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 16,
          "plid": 152553,
          "movetime": 1649098769881,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 17,
          "plid": 44616,
          "movetime": 1649129481459,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 18,
          "plid": 152553,
          "movetime": 1649186018829,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 19,
          "plid": 44616,
          "movetime": 1649207012462,
          "jmove": "fa",
          "dmove": "F1"
        },
        {
          "nmove": 20,
          "plid": 152553,
          "movetime": 1649270824545,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 21,
          "plid": 44616,
          "movetime": 1649294143396,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 22,
          "plid": 152553,
          "movetime": 1649355426528,
          "jmove": "ic",
          "dmove": "I3"
        },
        {
          "nmove": 23,
          "plid": 44616,
          "movetime": 1649359946755,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 24,
          "plid": 152553,
          "movetime": 1649510257588,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 25,
          "plid": 44616,
          "movetime": 1649562819739,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 26,
          "plid": 152553,
          "movetime": 1649584917578,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 27,
          "plid": 44616,
          "movetime": 1649638583030,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 28,
          "plid": 152553,
          "movetime": 1649788391343,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 29,
          "plid": 44616,
          "movetime": 1649895637417,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 30,
          "plid": 152553,
          "movetime": 1649961181046,
          "jmove": "fi",
          "dmove": "F9"
        },
        {
          "nmove": 31,
          "plid": 44616,
          "movetime": 1649980052653,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 32,
          "plid": 152553,
          "movetime": 1650042141628,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 33,
          "plid": 44616,
          "movetime": 1650061175993,
          "jmove": "ha",
          "dmove": "H1"
        },
        {
          "nmove": 34,
          "plid": 152553,
          "movetime": 1650116956969,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 35,
          "plid": 44616,
          "movetime": 1650154004922,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 36,
          "plid": 152553,
          "movetime": 1650218069498,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 37,
          "plid": 44616,
          "movetime": 1650331025514,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 38,
          "plid": 152553,
          "movetime": 1650391622085,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 39,
          "plid": 44616,
          "movetime": 1650424757144,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 40,
          "plid": 152553,
          "movetime": 1650478845689,
          "jmove": "ib",
          "dmove": "I2"
        },
        {
          "nmove": 41,
          "plid": 44616,
          "movetime": 1650501583800,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 42,
          "plid": 152553,
          "movetime": 1650565797953,
          "jmove": "ia",
          "dmove": "I1"
        },
        {
          "nmove": 43,
          "plid": 44616,
          "movetime": 1650631829896,
          "jmove": "ga",
          "dmove": "G1"
        },
        {
          "nmove": 44,
          "plid": 152553,
          "movetime": 1650739050263,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 45,
          "plid": 44616,
          "movetime": 1650809618246,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 46,
          "plid": 152553,
          "movetime": 1650824989067,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 47,
          "plid": 44616,
          "movetime": 1650942336590,
          "jmove": "score",
          "dmove": "Score"
        },
        {
          "nmove": 48,
          "plid": 152553,
          "movetime": 1650995238915,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302385,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 144760,
            "real_name": "galispiar",
            "membership": false,
            "country": "JP"
          },
          "rating": 1021.5246,
          "deviation": 20
        },
        {
          "player": {
            "plid": 44616,
            "real_name": "nullptr",
            "membership": false,
            "country": "US"
          },
          "rating": 1737.2621,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 144760,
      "expire_time": 1649749682601,
      "chngr": [
        -13.76901,
        4.831231
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685161,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 144760,
          "movetime": 1649154073104,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 2,
          "plid": 44616,
          "movetime": 1649206945755,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 3,
          "plid": 144760,
          "movetime": 1649401371729,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 4,
          "plid": 44616,
          "movetime": 1649429982606,
          "jmove": "dg",
          "dmove": "D7"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        230400000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302386,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 152553,
            "real_name": "pacmaniac",
            "membership": false,
            "country": "EU"
          },
          "rating": 1825.2876,
          "deviation": 31
        },
        {
          "player": {
            "plid": 4090,
            "real_name": "David Milne",
            "membership": true,
            "country": "NZ"
          },
          "rating": 1551.7124,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 0,
      "expire_time": 1651987376808,
      "chngr": [
        21.369265,
        -6.105504
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685163,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 152553,
          "movetime": 1648469123470,
          "jmove": "ff",
          "dmove": "F6"
        },
        {
          "nmove": 2,
          "plid": 4090,
          "movetime": 1648512482992,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 3,
          "plid": 152553,
          "movetime": 1648554947023,
          "jmove": "de",
          "dmove": "D5"
        },
        {
          "nmove": 4,
          "plid": 4090,
          "movetime": 1648600672375,
          "jmove": "cc",
          "dmove": "C3"
        },
        {
          "nmove": 5,
          "plid": 152553,
          "movetime": 1648649935215,
          "jmove": "ec",
          "dmove": "E3"
        },
        {
          "nmove": 6,
          "plid": 4090,
          "movetime": 1648689342480,
          "jmove": "gc",
          "dmove": "G3"
        },
        {
          "nmove": 7,
          "plid": 152553,
          "movetime": 1648742415626,
          "jmove": "cf",
          "dmove": "C6"
        },
        {
          "nmove": 8,
          "plid": 4090,
          "movetime": 1648802715776,
          "jmove": "gg",
          "dmove": "G7"
        },
        {
          "nmove": 9,
          "plid": 152553,
          "movetime": 1648817924063,
          "jmove": "fg",
          "dmove": "F7"
        },
        {
          "nmove": 10,
          "plid": 4090,
          "movetime": 1648862549045,
          "jmove": "fh",
          "dmove": "F8"
        },
        {
          "nmove": 11,
          "plid": 152553,
          "movetime": 1648898377917,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 12,
          "plid": 4090,
          "movetime": 1648960007674,
          "jmove": "hh",
          "dmove": "H8"
        },
        {
          "nmove": 13,
          "plid": 152553,
          "movetime": 1649011594229,
          "jmove": "hg",
          "dmove": "H7"
        },
        {
          "nmove": 14,
          "plid": 4090,
          "movetime": 1649061771874,
          "jmove": "gh",
          "dmove": "G8"
        },
        {
          "nmove": 15,
          "plid": 152553,
          "movetime": 1649098850582,
          "jmove": "eh",
          "dmove": "E8"
        },
        {
          "nmove": 16,
          "plid": 4090,
          "movetime": 1649121129368,
          "jmove": "eg",
          "dmove": "E7"
        },
        {
          "nmove": 17,
          "plid": 152553,
          "movetime": 1649185997170,
          "jmove": "dh",
          "dmove": "D8"
        },
        {
          "nmove": 18,
          "plid": 4090,
          "movetime": 1649209091909,
          "jmove": "ch",
          "dmove": "C8"
        },
        {
          "nmove": 19,
          "plid": 152553,
          "movetime": 1649270867862,
          "jmove": "bh",
          "dmove": "B8"
        },
        {
          "nmove": 20,
          "plid": 4090,
          "movetime": 1649290896711,
          "jmove": "cg",
          "dmove": "C7"
        },
        {
          "nmove": 21,
          "plid": 152553,
          "movetime": 1649355401740,
          "jmove": "bg",
          "dmove": "B7"
        },
        {
          "nmove": 22,
          "plid": 4090,
          "movetime": 1649378647063,
          "jmove": "di",
          "dmove": "D9"
        },
        {
          "nmove": 23,
          "plid": 152553,
          "movetime": 1649510302408,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 24,
          "plid": 4090,
          "movetime": 1649552939461,
          "jmove": "gb",
          "dmove": "G2"
        },
        {
          "nmove": 25,
          "plid": 152553,
          "movetime": 1649585052673,
          "jmove": "db",
          "dmove": "D2"
        },
        {
          "nmove": 26,
          "plid": 4090,
          "movetime": 1649643910644,
          "jmove": "cb",
          "dmove": "C2"
        },
        {
          "nmove": 27,
          "plid": 152553,
          "movetime": 1649788427612,
          "jmove": "he",
          "dmove": "H5"
        },
        {
          "nmove": 28,
          "plid": 4090,
          "movetime": 1649815938998,
          "jmove": "hd",
          "dmove": "H4"
        },
        {
          "nmove": 29,
          "plid": 152553,
          "movetime": 1649961118355,
          "jmove": "hb",
          "dmove": "H2"
        },
        {
          "nmove": 30,
          "plid": 4090,
          "movetime": 1650082340663,
          "jmove": "ha",
          "dmove": "H1"
        },
        {
          "nmove": 31,
          "plid": 152553,
          "movetime": 1650116931502,
          "jmove": "ib",
          "dmove": "I2"
        },
        {
          "nmove": 32,
          "plid": 4090,
          "movetime": 1650157743715,
          "jmove": "fb",
          "dmove": "F2"
        },
        {
          "nmove": 33,
          "plid": 152553,
          "movetime": 1650218110100,
          "jmove": "eb",
          "dmove": "E2"
        },
        {
          "nmove": 34,
          "plid": 4090,
          "movetime": 1650251610498,
          "jmove": "fa",
          "dmove": "F1"
        },
        {
          "nmove": 35,
          "plid": 152553,
          "movetime": 1650277623717,
          "jmove": "id",
          "dmove": "I4"
        },
        {
          "nmove": 36,
          "plid": 4090,
          "movetime": 1650324658045,
          "jmove": "be",
          "dmove": "B5"
        },
        {
          "nmove": 37,
          "plid": 152553,
          "movetime": 1650391598584,
          "jmove": "bf",
          "dmove": "B6"
        },
        {
          "nmove": 38,
          "plid": 4090,
          "movetime": 1650458297353,
          "jmove": "dd",
          "dmove": "D4"
        },
        {
          "nmove": 39,
          "plid": 152553,
          "movetime": 1650478901361,
          "jmove": "ed",
          "dmove": "E4"
        },
        {
          "nmove": 40,
          "plid": 4090,
          "movetime": 1650515293500,
          "jmove": "ce",
          "dmove": "C5"
        },
        {
          "nmove": 41,
          "plid": 152553,
          "movetime": 1650565893771,
          "jmove": "df",
          "dmove": "D6"
        },
        {
          "nmove": 42,
          "plid": 4090,
          "movetime": 1650593886858,
          "jmove": "ei",
          "dmove": "E9"
        },
        {
          "nmove": 43,
          "plid": 152553,
          "movetime": 1650738982668,
          "jmove": "ae",
          "dmove": "A5"
        },
        {
          "nmove": 44,
          "plid": 4090,
          "movetime": 1650766595972,
          "jmove": "bd",
          "dmove": "B4"
        },
        {
          "nmove": 45,
          "plid": 152553,
          "movetime": 1650784985918,
          "jmove": "ef",
          "dmove": "E6"
        },
        {
          "nmove": 46,
          "plid": 4090,
          "movetime": 1650857828017,
          "jmove": "ig",
          "dmove": "I7"
        },
        {
          "nmove": 47,
          "plid": 152553,
          "movetime": 1650908960620,
          "jmove": "hf",
          "dmove": "H6"
        },
        {
          "nmove": 48,
          "plid": 4090,
          "movetime": 1650945319094,
          "jmove": "fd",
          "dmove": "F4"
        },
        {
          "nmove": 49,
          "plid": 152553,
          "movetime": 1650995255030,
          "jmove": "da",
          "dmove": "D1"
        },
        {
          "nmove": 50,
          "plid": 4090,
          "movetime": 1651023575938,
          "jmove": "ca",
          "dmove": "C1"
        },
        {
          "nmove": 51,
          "plid": 152553,
          "movetime": 1651084983625,
          "jmove": "bi",
          "dmove": "B9"
        },
        {
          "nmove": 52,
          "plid": 4090,
          "movetime": 1651125777810,
          "jmove": "dc",
          "dmove": "D3"
        },
        {
          "nmove": 53,
          "plid": 152553,
          "movetime": 1651167798697,
          "jmove": "hc",
          "dmove": "H3"
        },
        {
          "nmove": 54,
          "plid": 4090,
          "movetime": 1651201484839,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 55,
          "plid": 152553,
          "movetime": 1651338523089,
          "jmove": "ge",
          "dmove": "G5"
        },
        {
          "nmove": 56,
          "plid": 4090,
          "movetime": 1651375174574,
          "jmove": "ad",
          "dmove": "A4"
        },
        {
          "nmove": 57,
          "plid": 152553,
          "movetime": 1651385063531,
          "jmove": "af",
          "dmove": "A6"
        },
        {
          "nmove": 58,
          "plid": 4090,
          "movetime": 1651395626229,
          "jmove": "ah",
          "dmove": "A8"
        },
        {
          "nmove": 59,
          "plid": 152553,
          "movetime": 1651428749667,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 60,
          "plid": 4090,
          "movetime": 1651456102090,
          "jmove": "if",
          "dmove": "I6"
        },
        {
          "nmove": 61,
          "plid": 152553,
          "movetime": 1651561348737,
          "jmove": "ie",
          "dmove": "I5"
        },
        {
          "nmove": 62,
          "plid": 4090,
          "movetime": 1651576671825,
          "jmove": "ih",
          "dmove": "I8"
        },
        {
          "nmove": 63,
          "plid": 152553,
          "movetime": 1651598915068,
          "jmove": "ic",
          "dmove": "I3"
        },
        {
          "nmove": 64,
          "plid": 4090,
          "movetime": 1651621178575,
          "jmove": "ci",
          "dmove": "C9"
        },
        {
          "nmove": 65,
          "plid": 152553,
          "movetime": 1651685864951,
          "jmove": "ba",
          "dmove": "B1"
        },
        {
          "nmove": 66,
          "plid": 4090,
          "movetime": 1651721061674,
          "jmove": "bb",
          "dmove": "B2"
        },
        {
          "nmove": 67,
          "plid": 152553,
          "movetime": 1651773879021,
          "jmove": "fe",
          "dmove": "F5"
        },
        {
          "nmove": 68,
          "plid": 4090,
          "movetime": 1651834753473,
          "jmove": "ag",
          "dmove": "A7"
        },
        {
          "nmove": 69,
          "plid": 152553,
          "movetime": 1651922887085,
          "jmove": "ia",
          "dmove": "I1"
        },
        {
          "nmove": 70,
          "plid": 4090,
          "movetime": 1651923599211,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 71,
          "plid": 152553,
          "movetime": 1651925391587,
          "jmove": "pass",
          "dmove": "Pass"
        },
        {
          "nmove": 72,
          "plid": 4090,
          "movetime": 1651981560381,
          "jmove": "scorebaaggb",
          "dmove": "Score"
        },
        {
          "nmove": 73,
          "plid": 152553,
          "movetime": 1651987376804,
          "jmove": "accept",
          "dmove": "Accept"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302387,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 4090,
            "real_name": "David Milne",
            "membership": true,
            "country": "NZ"
          },
          "rating": 1551.7124,
          "deviation": 20
        },
        {
          "player": {
            "plid": 144760,
            "real_name": "galispiar",
            "membership": false,
            "country": "JP"
          },
          "rating": 1021.5246,
          "deviation": 20
        }
      ],
      "status": 1,
      "results": [
        2,
        0
      ],
      "onmove": 144760,
      "expire_time": 1649749686669,
      "chngr": [
        5.3907814,
        -14.55511
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685165,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 4090,
          "movetime": 1648456047313,
          "jmove": "cd",
          "dmove": "C4"
        },
        {
          "nmove": 2,
          "plid": 144760,
          "movetime": 1649154118673,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 3,
          "plid": 4090,
          "movetime": 1649209015533,
          "jmove": "dg",
          "dmove": "D7"
        },
        {
          "nmove": 4,
          "plid": 144760,
          "movetime": 1649401451026,
          "jmove": "fc",
          "dmove": "F3"
        },
        {
          "nmove": 5,
          "plid": 4090,
          "movetime": 1649469210754,
          "jmove": "ee",
          "dmove": "E5"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        864000000,
        237600000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    },
    {
      "gid": 2302388,
      "gtid": "go19",
      "variant": "GO9",
      "players": [
        {
          "player": {
            "plid": 144760,
            "real_name": "galispiar",
            "membership": false,
            "country": "JP"
          },
          "rating": 1021.5246,
          "deviation": 20
        },
        {
          "player": {
            "plid": 152553,
            "real_name": "pacmaniac",
            "membership": false,
            "country": "EU"
          },
          "rating": 1825.2876,
          "deviation": 31
        }
      ],
      "status": 1,
      "results": [
        0,
        2
      ],
      "onmove": 144760,
      "expire_time": 1649749687417,
      "chngr": [
        -13.27092,
        19.781181
      ],
      "moves": [
        {
          "nmove": 0,
          "plid": 1,
          "movetime": 1648452685166,
          "jmove": "6.5|0",
          "dmove": ""
        },
        {
          "nmove": 1,
          "plid": 144760,
          "movetime": 1649154081471,
          "jmove": "ee",
          "dmove": "E5"
        },
        {
          "nmove": 2,
          "plid": 152553,
          "movetime": 1649186168285,
          "jmove": "gd",
          "dmove": "G4"
        },
        {
          "nmove": 3,
          "plid": 144760,
          "movetime": 1649401219735,
          "jmove": "gf",
          "dmove": "G6"
        },
        {
          "nmove": 4,
          "plid": 152553,
          "movetime": 1649510321705,
          "jmove": "ec",
          "dmove": "E3"
        }
      ],
      "messages": [],
      "ulid": "",
      "time": [
        212400000,
        864000000
      ],
      "points": [
        0,
        0
      ],
      "tournament": "cv",
      "trnid": "go19.cv.GO9.53.2.1"
    }
  ]
}
```