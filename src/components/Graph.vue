<template> 
    <Chart id = 'kl' containerClass='klchart' :data='data' @kl-ready='klReady'/>
</template>

<script>
import 'keylines';
import { Chart } from './vue-keylines';

export default {
    name: 'app',
    components: { Chart },
    methods: {

        klReady(chart) {
            this.chart = chart;
        },
    },
    data() {
        return{
            data: {
                pokedex: [{
    "1": {
        "name": "Bulbasaur",
        "type": {
            "1": "Grass",
            "2": "Poison"
        },
        "stats": {
            "hp": "45",
            "attack": "49",
            "defense": "49",
            "speed": "45",
            "special": "65"
        }
    },
    "2": {
        "name": "Ivysaur",
        "type": {
            "1": "Grass",
            "2": "Poison"
        },
        "stats": {
            "hp": "60",
            "attack": "62",
            "defense": "63",
            "speed": "60",
            "special": "80"
        }
    },
    "3": {
        "name": "Venusaur",
        "type": {
            "1": "Grass",
            "2": "Poison"
        },
        "stats": {
            "hp": "80",
            "attack": "82",
            "defense": "83",
            "speed": "80",
            "special": "100"
        }
    },
    "4": {
        "name": "Charmander",
        "type": {
            "1": "Fire",
            "2": ""
        },
        "stats": {
            "hp": "39",
            "attack": "52",
            "defense": "43",
            "speed": "65",
            "special": "50"
        }
    },
    "5": {
        "name": "Charmeleon",
        "type": {
            "1": "Fire",
            "2": ""
        },
        "stats": {
            "hp": "58",
            "attack": "64",
            "defense": "58",
            "speed": "80",
            "special": "65"
        }
    },
    "6": {
        "name": "Charizard",
        "type": {
            "1": "Fire",
            "2": "Flying"
        },
        "stats": {
            "hp": "78",
            "attack": "84",
            "defense": "78",
            "speed": "100",
            "special": "85"
        }
    },
    "7": {
        "name": "Squirtle",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "44",
            "attack": "48",
            "defense": "65",
            "speed": "43",
            "special": "50"
        }
    },
    "8": {
        "name": "Wartortle",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "59",
            "attack": "63",
            "defense": "80",
            "speed": "58",
            "special": "65"
        }
    },
    "9": {
        "name": "Blastoise",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "79",
            "attack": "83",
            "defense": "100",
            "speed": "78",
            "special": "85"
        }
    },
    "10": {
        "name": "Caterpie",
        "type": {
            "1": "Bug",
            "2": ""
        },
        "stats": {
            "hp": "45",
            "attack": "30",
            "defense": "35",
            "speed": "45",
            "special": "20"
        }
    },
    "11": {
        "name": "Metapod",
        "type": {
            "1": "Bug",
            "2": ""
        },
        "stats": {
            "hp": "50",
            "attack": "20",
            "defense": "55",
            "speed": "30",
            "special": "25"
        }
    },
    "12": {
        "name": "Butterfree",
        "type": {
            "1": "Bug",
            "2": "Flying"
        },
        "stats": {
            "hp": "60",
            "attack": "45",
            "defense": "50",
            "speed": "70",
            "special": "80"
        }
    },
    "13": {
        "name": "Weedle",
        "type": {
            "1": "Bug",
            "2": "Poison"
        },
        "stats": {
            "hp": "40",
            "attack": "35",
            "defense": "30",
            "speed": "50",
            "special": "20"
        }
    },
    "14": {
        "name": "Kakuna",
        "type": {
            "1": "Bug",
            "2": "Poison"
        },
        "stats": {
            "hp": "45",
            "attack": "25",
            "defense": "50",
            "speed": "35",
            "special": "25"
        }
    },
    "15": {
        "name": "Beedrill",
        "type": {
            "1": "Bug",
            "2": "Poison"
        },
        "stats": {
            "hp": "65",
            "attack": "80",
            "defense": "40",
            "speed": "75",
            "special": "45"
        }
    },
    "16": {
        "name": "Pidgey",
        "type": {
            "1": "Normal",
            "2": "Flying"
        },
        "stats": {
            "hp": "40",
            "attack": "45",
            "defense": "40",
            "speed": "56",
            "special": "35"
        }
    },
    "17": {
        "name": "Pidgeotto",
        "type": {
            "1": "Normal",
            "2": "Flying"
        },
        "stats": {
            "hp": "63",
            "attack": "60",
            "defense": "55",
            "speed": "71",
            "special": "50"
        }
    },
    "18": {
        "name": "Pidgeot",
        "type": {
            "1": "Normal",
            "2": "Flying"
        },
        "stats": {
            "hp": "83",
            "attack": "80",
            "defense": "75",
            "speed": "91",
            "special": "70"
        }
    },
    "19": {
        "name": "Rattata",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "30",
            "attack": "56",
            "defense": "35",
            "speed": "72",
            "special": "25"
        }
    },
    "20": {
        "name": "Raticate",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "55",
            "attack": "81",
            "defense": "60",
            "speed": "97",
            "special": "50"
        }
    },
    "21": {
        "name": "Spearow",
        "type": {
            "1": "Normal",
            "2": "Flying"
        },
        "stats": {
            "hp": "40",
            "attack": "60",
            "defense": "30",
            "speed": "70",
            "special": "31"
        }
    },
    "22": {
        "name": "Fearow",
        "type": {
            "1": "Normal",
            "2": "Flying"
        },
        "stats": {
            "hp": "65",
            "attack": "90",
            "defense": "65",
            "speed": "100",
            "special": "61"
        }
    },
    "23": {
        "name": "Ekans",
        "type": {
            "1": "Poison",
            "2": ""
        },
        "stats": {
            "hp": "35",
            "attack": "60",
            "defense": "44",
            "speed": "55",
            "special": "40"
        }
    },
    "24": {
        "name": "Arbok",
        "type": {
            "1": "Poison",
            "2": ""
        },
        "stats": {
            "hp": "60",
            "attack": "85",
            "defense": "69",
            "speed": "80",
            "special": "65"
        }
    },
    "25": {
        "name": "Pikachu",
        "type": {
            "1": "Electric",
            "2": ""
        },
        "stats": {
            "hp": "35",
            "attack": "55",
            "defense": "30",
            "speed": "90",
            "special": "50"
        }
    },
    "26": {
        "name": "Raichu",
        "type": {
            "1": "Electric",
            "2": ""
        },
        "stats": {
            "hp": "60",
            "attack": "90",
            "defense": "55",
            "speed": "100",
            "special": "90"
        }
    },
    "27": {
        "name": "Sandshrew",
        "type": {
            "1": "Ground",
            "2": ""
        },
        "stats": {
            "hp": "50",
            "attack": "75",
            "defense": "85",
            "speed": "40",
            "special": "30"
        }
    },
    "28": {
        "name": "Sandslash",
        "type": {
            "1": "Ground",
            "2": ""
        },
        "stats": {
            "hp": "75",
            "attack": "100",
            "defense": "110",
            "speed": "65",
            "special": "55"
        }
    },
    "29": {
        "name": "Nidoran♀",
        "type": {
            "1": "Poison",
            "2": ""
        },
        "stats": {
            "hp": "55",
            "attack": "47",
            "defense": "52",
            "speed": "41",
            "special": "40"
        }
    },
    "30": {
        "name": "Nidorina",
        "type": {
            "1": "Poison",
            "2": ""
        },
        "stats": {
            "hp": "70",
            "attack": "62",
            "defense": "67",
            "speed": "56",
            "special": "55"
        }
    },
    "31": {
        "name": "Nidoqueen",
        "type": {
            "1": "Poison",
            "2": "Ground"
        },
        "stats": {
            "hp": "90",
            "attack": "82",
            "defense": "87",
            "speed": "76",
            "special": "75"
        }
    },
    "32": {
        "name": "Nidoran♂",
        "type": {
            "1": "Poison",
            "2": ""
        },
        "stats": {
            "hp": "46",
            "attack": "57",
            "defense": "40",
            "speed": "50",
            "special": "40"
        }
    },
    "33": {
        "name": "Nidorino",
        "type": {
            "1": "Poison",
            "2": ""
        },
        "stats": {
            "hp": "61",
            "attack": "72",
            "defense": "57",
            "speed": "65",
            "special": "55"
        }
    },
    "34": {
        "name": "Nidoking",
        "type": {
            "1": "Poison",
            "2": "Ground"
        },
        "stats": {
            "hp": "81",
            "attack": "92",
            "defense": "77",
            "speed": "85",
            "special": "75"
        }
    },
    "35": {
        "name": "Clefairy",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "70",
            "attack": "45",
            "defense": "48",
            "speed": "35",
            "special": "60"
        }
    },
    "36": {
        "name": "Clefable",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "95",
            "attack": "70",
            "defense": "73",
            "speed": "60",
            "special": "85"
        }
    },
    "37": {
        "name": "Vulpix",
        "type": {
            "1": "Fire",
            "2": ""
        },
        "stats": {
            "hp": "38",
            "attack": "41",
            "defense": "40",
            "speed": "65",
            "special": "65"
        }
    },
    "38": {
        "name": "Ninetales",
        "type": {
            "1": "Fire",
            "2": ""
        },
        "stats": {
            "hp": "73",
            "attack": "76",
            "defense": "75",
            "speed": "100",
            "special": "100"
        }
    },
    "39": {
        "name": "Jigglypuff",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "115",
            "attack": "45",
            "defense": "20",
            "speed": "20",
            "special": "25"
        }
    },
    "40": {
        "name": "Wigglytuff",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "140",
            "attack": "70",
            "defense": "45",
            "speed": "45",
            "special": "50"
        }
    },
    "41": {
        "name": "Zubat",
        "type": {
            "1": "Poison",
            "2": "Flying"
        },
        "stats": {
            "hp": "40",
            "attack": "45",
            "defense": "35",
            "speed": "55",
            "special": "40"
        }
    },
    "42": {
        "name": "Golbat",
        "type": {
            "1": "Poison",
            "2": "Flying"
        },
        "stats": {
            "hp": "75",
            "attack": "80",
            "defense": "70",
            "speed": "90",
            "special": "75"
        }
    },
    "43": {
        "name": "Oddish",
        "type": {
            "1": "Grass",
            "2": "Poison"
        },
        "stats": {
            "hp": "45",
            "attack": "50",
            "defense": "55",
            "speed": "30",
            "special": "75"
        }
    },
    "44": {
        "name": "Gloom",
        "type": {
            "1": "Grass",
            "2": "Poison"
        },
        "stats": {
            "hp": "60",
            "attack": "65",
            "defense": "70",
            "speed": "40",
            "special": "85"
        }
    },
    "45": {
        "name": "Vileplume",
        "type": {
            "1": "Grass",
            "2": "Poison"
        },
        "stats": {
            "hp": "75",
            "attack": "80",
            "defense": "85",
            "speed": "50",
            "special": "100"
        }
    },
    "46": {
        "name": "Paras",
        "type": {
            "1": "Bug",
            "2": "Grass"
        },
        "stats": {
            "hp": "35",
            "attack": "70",
            "defense": "55",
            "speed": "25",
            "special": "55"
        }
    },
    "47": {
        "name": "Parasect",
        "type": {
            "1": "Bug",
            "2": "Grass"
        },
        "stats": {
            "hp": "60",
            "attack": "95",
            "defense": "80",
            "speed": "30",
            "special": "80"
        }
    },
    "48": {
        "name": "Venonat",
        "type": {
            "1": "Bug",
            "2": "Poison"
        },
        "stats": {
            "hp": "60",
            "attack": "55",
            "defense": "50",
            "speed": "45",
            "special": "40"
        }
    },
    "49": {
        "name": "Venomoth",
        "type": {
            "1": "Bug",
            "2": "Poison"
        },
        "stats": {
            "hp": "70",
            "attack": "65",
            "defense": "60",
            "speed": "90",
            "special": "90"
        }
    },
    "50": {
        "name": "Diglett",
        "type": {
            "1": "Ground",
            "2": ""
        },
        "stats": {
            "hp": "10",
            "attack": "55",
            "defense": "25",
            "speed": "95",
            "special": "45"
        }
    },
    "51": {
        "name": "Dugtrio",
        "type": {
            "1": "Ground",
            "2": ""
        },
        "stats": {
            "hp": "35",
            "attack": "80",
            "defense": "50",
            "speed": "120",
            "special": "70"
        }
    },
    "52": {
        "name": "Meowth",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "40",
            "attack": "45",
            "defense": "35",
            "speed": "90",
            "special": "40"
        }
    },
    "53": {
        "name": "Persian",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "65",
            "attack": "70",
            "defense": "60",
            "speed": "115",
            "special": "65"
        }
    },
    "54": {
        "name": "Psyduck",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "50",
            "attack": "52",
            "defense": "48",
            "speed": "55",
            "special": "50"
        }
    },
    "55": {
        "name": "Golduck",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "80",
            "attack": "82",
            "defense": "78",
            "speed": "85",
            "special": "80"
        }
    },
    "56": {
        "name": "Mankey",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "40",
            "attack": "80",
            "defense": "35",
            "speed": "70",
            "special": "35"
        }
    },
    "57": {
        "name": "Primeape",
        "type": {
            "1": "Fighting",
            "2": ""
        },
        "stats": {
            "hp": "65",
            "attack": "105",
            "defense": "60",
            "speed": "95",
            "special": "60"
        }
    },
    "58": {
        "name": "Growlithe",
        "type": {
            "1": "Fighting",
            "2": ""
        },
        "stats": {
            "hp": "55",
            "attack": "70",
            "defense": "45",
            "speed": "60",
            "special": "50"
        }
    },
    "59": {
        "name": "Arcanine",
        "type": {
            "1": "Fire",
            "2": ""
        },
        "stats": {
            "hp": "90",
            "attack": "110",
            "defense": "80",
            "speed": "95",
            "special": "80"
        }
    },
    "60": {
        "name": "Poliwag",
        "type": {
            "1": "Fire",
            "2": ""
        },
        "stats": {
            "hp": "40",
            "attack": "50",
            "defense": "40",
            "speed": "90",
            "special": "40"
        }
    },
    "61": {
        "name": "Poliwhirl",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "65",
            "attack": "65",
            "defense": "65",
            "speed": "90",
            "special": "50"
        }
    },
    "62": {
        "name": "Poliwrath",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "90",
            "attack": "85",
            "defense": "95",
            "speed": "70",
            "special": "70"
        }
    },
    "63": {
        "name": "Abra",
        "type": {
            "1": "Water",
            "2": "Fighting"
        },
        "stats": {
            "hp": "25",
            "attack": "20",
            "defense": "15",
            "speed": "90",
            "special": "105"
        }
    },
    "64": {
        "name": "Kadabra",
        "type": {
            "1": "Psychic",
            "2": ""
        },
        "stats": {
            "hp": "40",
            "attack": "35",
            "defense": "30",
            "speed": "105",
            "special": "120"
        }
    },
    "65": {
        "name": "Alakazam",
        "type": {
            "1": "Psychic",
            "2": ""
        },
        "stats": {
            "hp": "55",
            "attack": "50",
            "defense": "45",
            "speed": "120",
            "special": "135"
        }
    },
    "66": {
        "name": "Machop",
        "type": {
            "1": "Psychic",
            "2": ""
        },
        "stats": {
            "hp": "70",
            "attack": "80",
            "defense": "50",
            "speed": "35",
            "special": "35"
        }
    },
    "67": {
        "name": "Machoke",
        "type": {
            "1": "Fighting",
            "2": ""
        },
        "stats": {
            "hp": "80",
            "attack": "100",
            "defense": "70",
            "speed": "45",
            "special": "50"
        }
    },
    "68": {
        "name": "Machamp",
        "type": {
            "1": "Fighting",
            "2": ""
        },
        "stats": {
            "hp": "90",
            "attack": "130",
            "defense": "80",
            "speed": "55",
            "special": "65"
        }
    },
    "69": {
        "name": "Bellsprout",
        "type": {
            "1": "Fighting",
            "2": ""
        },
        "stats": {
            "hp": "50",
            "attack": "75",
            "defense": "35",
            "speed": "40",
            "special": "70"
        }
    },
    "70": {
        "name": "Weepinbell",
        "type": {
            "1": "Grass",
            "2": "Poison"
        },
        "stats": {
            "hp": "65",
            "attack": "90",
            "defense": "50",
            "speed": "55",
            "special": "85"
        }
    },
    "71": {
        "name": "Victreebel",
        "type": {
            "1": "Grass",
            "2": "Poison"
        },
        "stats": {
            "hp": "80",
            "attack": "105",
            "defense": "65",
            "speed": "70",
            "special": "100"
        }
    },
    "72": {
        "name": "Tentacool",
        "type": {
            "1": "Grass",
            "2": "Poison"
        },
        "stats": {
            "hp": "40",
            "attack": "40",
            "defense": "35",
            "speed": "70",
            "special": "100"
        }
    },
    "73": {
        "name": "Tentacruel",
        "type": {
            "1": "Water",
            "2": "Poison"
        },
        "stats": {
            "hp": "80",
            "attack": "70",
            "defense": "65",
            "speed": "100",
            "special": "120"
        }
    },
    "74": {
        "name": "Geodude",
        "type": {
            "1": "Water",
            "2": "Poison"
        },
        "stats": {
            "hp": "40",
            "attack": "80",
            "defense": "100",
            "speed": "20",
            "special": "30"
        }
    },
    "75": {
        "name": "Graveler",
        "type": {
            "1": "Rock",
            "2": "Ground"
        },
        "stats": {
            "hp": "55",
            "attack": "95",
            "defense": "115",
            "speed": "35",
            "special": "45"
        }
    },
    "76": {
        "name": "Golem",
        "type": {
            "1": "Rock",
            "2": "Ground"
        },
        "stats": {
            "hp": "80",
            "attack": "110",
            "defense": "130",
            "speed": "45",
            "special": "55"
        }
    },
    "77": {
        "name": "Ponyta",
        "type": {
            "1": "Rock",
            "2": "Ground"
        },
        "stats": {
            "hp": "50",
            "attack": "85",
            "defense": "55",
            "speed": "90",
            "special": "65"
        }
    },
    "78": {
        "name": "Rapidash",
        "type": {
            "1": "Fire",
            "2": ""
        },
        "stats": {
            "hp": "65",
            "attack": "100",
            "defense": "70",
            "speed": "105",
            "special": "80"
        }
    },
    "79": {
        "name": "Slowpoke",
        "type": {
            "1": "Fire",
            "2": ""
        },
        "stats": {
            "hp": "90",
            "attack": "65",
            "defense": "65",
            "speed": "15",
            "special": "40"
        }
    },
    "80": {
        "name": "Slowbro",
        "type": {
            "1": "Water",
            "2": "Psychic"
        },
        "stats": {
            "hp": "95",
            "attack": "75",
            "defense": "110",
            "speed": "30",
            "special": "80"
        }
    },
    "81": {
        "name": "Magnemite",
        "type": {
            "1": "Water",
            "2": "Psychic"
        },
        "stats": {
            "hp": "25",
            "attack": "35",
            "defense": "70",
            "speed": "45",
            "special": "95"
        }
    },
    "82": {
        "name": "Magneton",
        "type": {
            "1": "Electric",
            "2": "Steel"
        },
        "stats": {
            "hp": "50",
            "attack": "60",
            "defense": "95",
            "speed": "70",
            "special": "120"
        }
    },
    "83": {
        "name": "Farfetch'd",
        "type": {
            "1": "Electric",
            "2": "Steel"
        },
        "stats": {
            "hp": "52",
            "attack": "65",
            "defense": "55",
            "speed": "60",
            "special": "58"
        }
    },
    "84": {
        "name": "Doduo",
        "type": {
            "1": "Normal",
            "2": "Flying"
        },
        "stats": {
            "hp": "35",
            "attack": "85",
            "defense": "45",
            "speed": "75",
            "special": "35"
        }
    },
    "85": {
        "name": "Dodrio",
        "type": {
            "1": "Normal",
            "2": "Flying"
        },
        "stats": {
            "hp": "60",
            "attack": "110",
            "defense": "70",
            "speed": "100",
            "special": "60"
        }
    },
    "86": {
        "name": "Seel",
        "type": {
            "1": "Normal",
            "2": "Flying"
        },
        "stats": {
            "hp": "65",
            "attack": "45",
            "defense": "55",
            "speed": "45",
            "special": "70"
        }
    },
    "87": {
        "name": "Dewgong",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "90",
            "attack": "70",
            "defense": "80",
            "speed": "70",
            "special": "95"
        }
    },
    "88": {
        "name": "Grimer",
        "type": {
            "1": "Water",
            "2": "Ice"
        },
        "stats": {
            "hp": "80",
            "attack": "80",
            "defense": "50",
            "speed": "25",
            "special": "40"
        }
    },
    "89": {
        "name": "Muk",
        "type": {
            "1": "Poison",
            "2": ""
        },
        "stats": {
            "hp": "105",
            "attack": "105",
            "defense": "75",
            "speed": "50",
            "special": "65"
        }
    },
    "90": {
        "name": "Shellder",
        "type": {
            "1": "Poison",
            "2": ""
        },
        "stats": {
            "hp": "30",
            "attack": "65",
            "defense": "100",
            "speed": "40",
            "special": "45"
        }
    },
    "91": {
        "name": "Cloyster",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "50",
            "attack": "95",
            "defense": "180",
            "speed": "70",
            "special": "85"
        }
    },
    "92": {
        "name": "Gastly",
        "type": {
            "1": "Water",
            "2": "Ice"
        },
        "stats": {
            "hp": "30",
            "attack": "35",
            "defense": "30",
            "speed": "80",
            "special": "100"
        }
    },
    "93": {
        "name": "Haunter",
        "type": {
            "1": "Ghost",
            "2": "Poison"
        },
        "stats": {
            "hp": "45",
            "attack": "50",
            "defense": "45",
            "speed": "95",
            "special": "115"
        }
    },
    "94": {
        "name": "Gengar",
        "type": {
            "1": "Ghost",
            "2": "Poison"
        },
        "stats": {
            "hp": "60",
            "attack": "65",
            "defense": "60",
            "speed": "110",
            "special": "130"
        }
    },
    "95": {
        "name": "Onix",
        "type": {
            "1": "Ghost",
            "2": "Poison"
        },
        "stats": {
            "hp": "35",
            "attack": "45",
            "defense": "160",
            "speed": "70",
            "special": "30"
        }
    },
    "96": {
        "name": "Drowzee",
        "type": {
            "1": "Rock",
            "2": "Ground"
        },
        "stats": {
            "hp": "60",
            "attack": "48",
            "defense": "45",
            "speed": "42",
            "special": "90"
        }
    },
    "97": {
        "name": "Hypno",
        "type": {
            "1": "Psychic",
            "2": ""
        },
        "stats": {
            "hp": "85",
            "attack": "73",
            "defense": "70",
            "speed": "67",
            "special": "115"
        }
    },
    "98": {
        "name": "Krabby",
        "type": {
            "1": "Psychic",
            "2": ""
        },
        "stats": {
            "hp": "30",
            "attack": "105",
            "defense": "90",
            "speed": "50",
            "special": "25"
        }
    },
    "99": {
        "name": "Kingler",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "55",
            "attack": "130",
            "defense": "115",
            "speed": "75",
            "special": "50"
        }
    },
    "100": {
        "name": "Voltorb",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "40",
            "attack": "30",
            "defense": "50",
            "speed": "100",
            "special": "55"
        }
    },
    "101": {
        "name": "Electrode",
        "type": {
            "1": "Electric",
            "2": ""
        },
        "stats": {
            "hp": "60",
            "attack": "50",
            "defense": "70",
            "speed": "140",
            "special": "80"
        }
    },
    "102": {
        "name": "Exeggcute",
        "type": {
            "1": "Electric",
            "2": ""
        },
        "stats": {
            "hp": "60",
            "attack": "40",
            "defense": "80",
            "speed": "40",
            "special": "60"
        }
    },
    "103": {
        "name": "Exeggutor",
        "type": {
            "1": "Grass",
            "2": "Psychic"
        },
        "stats": {
            "hp": "95",
            "attack": "95",
            "defense": "85",
            "speed": "55",
            "special": "125"
        }
    },
    "104": {
        "name": "Cubone",
        "type": {
            "1": "Grass",
            "2": "Psychic"
        },
        "stats": {
            "hp": "50",
            "attack": "50",
            "defense": "95",
            "speed": "35",
            "special": "40"
        }
    },
    "105": {
        "name": "Marowak",
        "type": {
            "1": "Ground",
            "2": ""
        },
        "stats": {
            "hp": "60",
            "attack": "80",
            "defense": "110",
            "speed": "45",
            "special": "50"
        }
    },
    "106": {
        "name": "Hitmonlee",
        "type": {
            "1": "Ground",
            "2": ""
        },
        "stats": {
            "hp": "50",
            "attack": "120",
            "defense": "53",
            "speed": "87",
            "special": "35"
        }
    },
    "107": {
        "name": "Hitmonchan",
        "type": {
            "1": "Fighting",
            "2": ""
        },
        "stats": {
            "hp": "50",
            "attack": "105",
            "defense": "79",
            "speed": "76",
            "special": "35"
        }
    },
    "108": {
        "name": "Lickitung",
        "type": {
            "1": "Fighting",
            "2": ""
        },
        "stats": {
            "hp": "90",
            "attack": "55",
            "defense": "75",
            "speed": "30",
            "special": "60"
        }
    },
    "109": {
        "name": "Koffing",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "40",
            "attack": "65",
            "defense": "95",
            "speed": "35",
            "special": "60"
        }
    },
    "110": {
        "name": "Weezing",
        "type": {
            "1": "Poison",
            "2": ""
        },
        "stats": {
            "hp": "65",
            "attack": "90",
            "defense": "120",
            "speed": "60",
            "special": "85"
        }
    },
    "111": {
        "name": "Rhyhorn",
        "type": {
            "1": "Poison",
            "2": ""
        },
        "stats": {
            "hp": "80",
            "attack": "85",
            "defense": "95",
            "speed": "25",
            "special": "30"
        }
    },
    "112": {
        "name": "Rhydon",
        "type": {
            "1": "Ground",
            "2": "Rock"
        },
        "stats": {
            "hp": "105",
            "attack": "130",
            "defense": "120",
            "speed": "40",
            "special": "45"
        }
    },
    "113": {
        "name": "Chansey",
        "type": {
            "1": "Ground",
            "2": "Rock"
        },
        "stats": {
            "hp": "250",
            "attack": "5",
            "defense": "5",
            "speed": "50",
            "special": "105"
        }
    },
    "114": {
        "name": "Tangela",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "65",
            "attack": "55",
            "defense": "115",
            "speed": "60",
            "special": "100"
        }
    },
    "115": {
        "name": "Kangaskhan",
        "type": {
            "1": "Grass",
            "2": ""
        },
        "stats": {
            "hp": "105",
            "attack": "95",
            "defense": "80",
            "speed": "90",
            "special": "40"
        }
    },
    "116": {
        "name": "Horsea",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "30",
            "attack": "40",
            "defense": "70",
            "speed": "60",
            "special": "70"
        }
    },
    "117": {
        "name": "Seadra",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "55",
            "attack": "65",
            "defense": "95",
            "speed": "85",
            "special": "95"
        }
    },
    "118": {
        "name": "Goldeen",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "45",
            "attack": "67",
            "defense": "60",
            "speed": "63",
            "special": "50"
        }
    },
    "119": {
        "name": "Seaking",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "80",
            "attack": "92",
            "defense": "65",
            "speed": "68",
            "special": "80"
        }
    },
    "120": {
        "name": "Staryu",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "30",
            "attack": "45",
            "defense": "55",
            "speed": "85",
            "special": "70"
        }
    },
    "121": {
        "name": "Starmie",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "60",
            "attack": "75",
            "defense": "85",
            "speed": "115",
            "special": "100"
        }
    },
    "122": {
        "name": "Mr. Mime",
        "type": {
            "1": "Water",
            "2": "Psychic"
        },
        "stats": {
            "hp": "40",
            "attack": "45",
            "defense": "65",
            "speed": "90",
            "special": "100"
        }
    },
    "123": {
        "name": "Scyther",
        "type": {
            "1": "Psychic",
            "2": ""
        },
        "stats": {
            "hp": "70",
            "attack": "110",
            "defense": "80",
            "speed": "105",
            "special": "55"
        }
    },
    "124": {
        "name": "Jynx",
        "type": {
            "1": "Bug",
            "2": "Flying"
        },
        "stats": {
            "hp": "65",
            "attack": "50",
            "defense": "35",
            "speed": "95",
            "special": "95"
        }
    },
    "125": {
        "name": "Electabuzz",
        "type": {
            "1": "Ice",
            "2": "Psychic"
        },
        "stats": {
            "hp": "65",
            "attack": "83",
            "defense": "57",
            "speed": "105",
            "special": "85"
        }
    },
    "126": {
        "name": "Magmar",
        "type": {
            "1": "Electric",
            "2": ""
        },
        "stats": {
            "hp": "65",
            "attack": "95",
            "defense": "57",
            "speed": "93",
            "special": "85"
        }
    },
    "127": {
        "name": "Pinsir",
        "type": {
            "1": "Fire",
            "2": ""
        },
        "stats": {
            "hp": "65",
            "attack": "125",
            "defense": "100",
            "speed": "85",
            "special": "55"
        }
    },
    "128": {
        "name": "Tauros",
        "type": {
            "1": "Bug",
            "2": ""
        },
        "stats": {
            "hp": "75",
            "attack": "100",
            "defense": "95",
            "speed": "110",
            "special": "70"
        }
    },
    "129": {
        "name": "Magikarp",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "20",
            "attack": "10",
            "defense": "55",
            "speed": "80",
            "special": "20"
        }
    },
    "130": {
        "name": "Gyarados",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "95",
            "attack": "125",
            "defense": "79",
            "speed": "81",
            "special": "100"
        }
    },
    "131": {
        "name": "Lapras",
        "type": {
            "1": "Water",
            "2": "Flying"
        },
        "stats": {
            "hp": "130",
            "attack": "85",
            "defense": "80",
            "speed": "60",
            "special": "95"
        }
    },
    "132": {
        "name": "Ditto",
        "type": {
            "1": "Water",
            "2": "Ice"
        },
        "stats": {
            "hp": "48",
            "attack": "48",
            "defense": "48",
            "speed": "48",
            "special": "48"
        }
    },
    "133": {
        "name": "Eevee",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "55",
            "attack": "55",
            "defense": "50",
            "speed": "55",
            "special": "65"
        }
    },
    "134": {
        "name": "Vaporeon",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "130",
            "attack": "65",
            "defense": "60",
            "speed": "65",
            "special": "110"
        }
    },
    "135": {
        "name": "Jolteon",
        "type": {
            "1": "Water",
            "2": ""
        },
        "stats": {
            "hp": "65",
            "attack": "65",
            "defense": "60",
            "speed": "130",
            "special": "110"
        }
    },
    "136": {
        "name": "Flareon",
        "type": {
            "1": "Electric",
            "2": ""
        },
        "stats": {
            "hp": "65",
            "attack": "130",
            "defense": "60",
            "speed": "65",
            "special": "110"
        }
    },
    "137": {
        "name": "Porygon",
        "type": {
            "1": "Fire",
            "2": ""
        },
        "stats": {
            "hp": "65",
            "attack": "60",
            "defense": "70",
            "speed": "40",
            "special": "75"
        }
    },
    "138": {
        "name": "Omanyte",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "35",
            "attack": "40",
            "defense": "100",
            "speed": "35",
            "special": "90"
        }
    },
    "139": {
        "name": "Omastar",
        "type": {
            "1": "Rock",
            "2": "Water"
        },
        "stats": {
            "hp": "70",
            "attack": "60",
            "defense": "125",
            "speed": "55",
            "special": "115"
        }
    },
    "140": {
        "name": "Kabuto",
        "type": {
            "1": "Rock",
            "2": "Water"
        },
        "stats": {
            "hp": "30",
            "attack": "80",
            "defense": "90",
            "speed": "55",
            "special": "45"
        }
    },
    "141": {
        "name": "Kabutops",
        "type": {
            "1": "Rock",
            "2": "Water"
        },
        "stats": {
            "hp": "60",
            "attack": "115",
            "defense": "105",
            "speed": "80",
            "special": "70"
        }
    },
    "142": {
        "name": "Aerodactyl",
        "type": {
            "1": "Rock",
            "2": "Water"
        },
        "stats": {
            "hp": "80",
            "attack": "105",
            "defense": "65",
            "speed": "130",
            "special": "60"
        }
    },
    "143": {
        "name": "Snorlax",
        "type": {
            "1": "Rock",
            "2": "Flying"
        },
        "stats": {
            "hp": "160",
            "attack": "110",
            "defense": "65",
            "speed": "30",
            "special": "65"
        }
    },
    "144": {
        "name": "Articuno",
        "type": {
            "1": "Normal",
            "2": ""
        },
        "stats": {
            "hp": "90",
            "attack": "85",
            "defense": "100",
            "speed": "85",
            "special": "125"
        }
    },
    "145": {
        "name": "Zapdos",
        "type": {
            "1": "Ice",
            "2": "Flying"
        },
        "stats": {
            "hp": "90",
            "attack": "90",
            "defense": "85",
            "speed": "100",
            "special": "125"
        }
    },
    "146": {
        "name": "Moltres",
        "type": {
            "1": "Electric",
            "2": "Flying"
        },
        "stats": {
            "hp": "90",
            "attack": "100",
            "defense": "90",
            "speed": "90",
            "special": "125"
        }
    },
    "147": {
        "name": "Dratini",
        "type": {
            "1": "Fire",
            "2": "Flying"
        },
        "stats": {
            "hp": "41",
            "attack": "64",
            "defense": "45",
            "speed": "50",
            "special": "50"
        }
    },
    "148": {
        "name": "Dragonair",
        "type": {
            "1": "Dragon",
            "2": ""
        },
        "stats": {
            "hp": "61",
            "attack": "84",
            "defense": "65",
            "speed": "70",
            "special": "70"
        }
    },
    "149": {
        "name": "Dragonite",
        "type": {
            "1": "Dragon",
            "2": ""
        },
        "stats": {
            "hp": "91",
            "attack": "134",
            "defense": "95",
            "speed": "80",
            "special": "100"
        }
    },
    "150": {
        "name": "Mewtwo",
        "type": {
            "1": "Dragon",
            "2": "Flying"
        },
        "stats": {
            "hp": "106",
            "attack": "110",
            "defense": "90",
            "speed": "130",
            "special": "154"
        }
    },
    "151": {
        "name": "Mew",
        "type": {
            "1": "Psychic",
            "2": ""
        },
        "stats": {
            "hp": "100",
            "attack": "100",
            "defense": "100",
            "speed": "100",
            "special": "100"
        }
    }
}],
  type: 'LinkChart',
  items: [
    { type: 'node', id: 'Bug', t: 'Bug' },
    { type: 'node', id: 'Dragon', t: 'Dragon' },
    { type: 'node', id: 'Electric', t: 'Electric' },
    { type: 'node', id: 'Fighting', t: 'Fighting' },
    { type: 'node', id: 'Fire', t: 'Fire' },
    { type: 'node', id: 'Flying', t: 'Flying' },
    { type: 'node', id: 'Ghost', t: 'Ghost' },
    { type: 'node', id: 'Grass', t: 'Grass' },
    { type: 'node', id: 'Ground', t: 'Ground' },
    { type: 'node', id: 'Ice', t: 'Ice' },
    { type: 'node', id: 'Normal', t: 'Normal' },
    { type: 'node', id: 'Poison', t: 'Poison' },
    { type: 'node', id: 'Psychic', t: 'Psychic' },
    { type: 'node', id: 'Rock', t: 'Rock' },
    { type: 'node', id: 'Water', t: 'Water' },
  ]
}
        }
    },
    mounted() {
        for(let index in this.data.pokedex[0]){
            this.data.items.push({type: 'node', id: this.data.pokedex[0][index].name, u: 'icons/pokeball.png', t: this.data.pokedex[0][index].name})
            this.data.items.push({type: 'link', id: index, id1: this.data.pokedex[0][index].name, id2: this.data.pokedex[0][index].type[1], a1: true, c: '#BD3B3B', w: 5})
            this.data.items.push({type: 'link', id: index + 151, id1: this.data.pokedex[0][index].name, id2: this.data.pokedex[0][index].type[2], a1: true, c: '#377FC3', w: 5})

        }
  },
}
</script>

<style>
.klchart{
    width: 100vw;
    height: 100vw;
}
</style>

