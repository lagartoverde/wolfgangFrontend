<template>
  <div class="table-container">
    <b-table 
      class='table' 
      striped 
      hover 
      :items="items" 
      :fields="fields"
      :sort-by.sync="sortBy"
      :sort-desc.sync="sortDesc"
    />
  </div>
</template>

<script>
  export default {
    data() {
      return {
        sortBy: 'name',
        sortDesc: false,
        fields: [
          { key: 'name', sortable: true },
          { key: 'role', sortable: true },
          { key: 'league', sortable: true },
          { key: 'trophies', sortable: true },
          { key: 'donations', sortable: true },
          { key: 'donationsReceived', sortable: true },
        ],
        items: [
          {
              "name": "@@@Bibek@@@",
              "role": "admin",
              "league": "Legend League",
              "trophies": 5121,
              "donations": 1852,
              "donationsReceived": 2483
          },
          {
              "name": "ymre",
              "role": "leader",
              "league": "Titan League I",
              "trophies": 4968,
              "donations": 5575,
              "donationsReceived": 3380
          },
          {
              "name": "phum12",
              "role": "coLeader",
              "league": "Titan League I",
              "trophies": 4876,
              "donations": 590,
              "donationsReceived": 2865
          },
          {
              "name": "Singledrop",
              "role": "coLeader",
              "league": "Unranked",
              "trophies": 4558,
              "donations": 0,
              "donationsReceived": 124
          },
          {
              "name": "scrubby",
              "role": "member",
              "league": "Titan League III",
              "trophies": 4323,
              "donations": 670,
              "donationsReceived": 1285
          },
          {
              "name": "Akeno",
              "role": "coLeader",
              "league": "Titan League III",
              "trophies": 4241,
              "donations": 285,
              "donationsReceived": 282
          },
          {
              "name": "crumblez",
              "role": "member",
              "league": "Titan League III",
              "trophies": 4150,
              "donations": 1262,
              "donationsReceived": 1209
          },
          {
              "name": "Dominik_DoDo",
              "role": "coLeader",
              "league": "Titan League III",
              "trophies": 4102,
              "donations": 1436,
              "donationsReceived": 606
          },
          {
              "name": "Bersih3.0",
              "role": "coLeader",
              "league": "Titan League III",
              "trophies": 4079,
              "donations": 152,
              "donationsReceived": 317
          },
          {
              "name": "Jack Kenoff",
              "role": "admin",
              "league": "Champion League II",
              "trophies": 3539,
              "donations": 60,
              "donationsReceived": 655
          },
          {
              "name": "Dig",
              "role": "member",
              "league": "Champion League II",
              "trophies": 3526,
              "donations": 198,
              "donationsReceived": 3029
          },
          {
              "name": "iAteUrDog69",
              "role": "member",
              "league": "Champion League II",
              "trophies": 3486,
              "donations": 0,
              "donationsReceived": 0
          },
          {
              "name": "LastOfManny",
              "role": "coLeader",
              "league": "Champion League III",
              "trophies": 3475,
              "donations": 1265,
              "donationsReceived": 1177
          },
          {
              "name": "Junior",
              "role": "member",
              "league": "Master League I",
              "trophies": 3161,
              "donations": 197,
              "donationsReceived": 402
          },
          {
              "name": "⭕️SvnthCircle⭕️",
              "role": "member",
              "league": "Master League I",
              "trophies": 3157,
              "donations": 1859,
              "donationsReceived": 0
          },
          {
              "name": "~Titanium~",
              "role": "member",
              "league": "Master League I",
              "trophies": 3127,
              "donations": 132,
              "donationsReceived": 138
          },
          {
              "name": "Law",
              "role": "admin",
              "league": "Master League II",
              "trophies": 2977,
              "donations": 481,
              "donationsReceived": 955
          },
          {
              "name": "Khaleesi",
              "role": "admin",
              "league": "Master League I",
              "trophies": 2977,
              "donations": 5010,
              "donationsReceived": 487
          },
          {
              "name": "Nerevar",
              "role": "admin",
              "league": "Master League II",
              "trophies": 2920,
              "donations": 75,
              "donationsReceived": 407
          },
          {
              "name": "eff-kha",
              "role": "coLeader",
              "league": "Master League II",
              "trophies": 2865,
              "donations": 178,
              "donationsReceived": 891
          },
          {
              "name": "DJ Thunder",
              "role": "member",
              "league": "Master League II",
              "trophies": 2798,
              "donations": 159,
              "donationsReceived": 441
          },
          {
              "name": "SmallAsianBoi",
              "role": "member",
              "league": "Master League II",
              "trophies": 2793,
              "donations": 0,
              "donationsReceived": 862
          },
          {
              "name": "~~OpT!C~~",
              "role": "admin",
              "league": "Master League III",
              "trophies": 2792,
              "donations": 45,
              "donationsReceived": 76
          },
          {
              "name": "BAISHYA",
              "role": "admin",
              "league": "Master League III",
              "trophies": 2767,
              "donations": 33,
              "donationsReceived": 105
          },
          {
              "name": "东方不败",
              "role": "member",
              "league": "Master League II",
              "trophies": 2747,
              "donations": 23,
              "donationsReceived": 107
          },
          {
              "name": "bchong",
              "role": "coLeader",
              "league": "Master League III",
              "trophies": 2740,
              "donations": 1308,
              "donationsReceived": 236
          },
          {
              "name": "_#LucifeR#_",
              "role": "admin",
              "league": "Master League II",
              "trophies": 2710,
              "donations": 1307,
              "donationsReceived": 1547
          },
          {
              "name": "Sai",
              "role": "member",
              "league": "Master League III",
              "trophies": 2656,
              "donations": 35,
              "donationsReceived": 0
          },
          {
              "name": "Sanjeet Deshwal",
              "role": "member",
              "league": "Master League III",
              "trophies": 2653,
              "donations": 236,
              "donationsReceived": 535
          },
          {
              "name": "mayusatko",
              "role": "member",
              "league": "Master League III",
              "trophies": 2630,
              "donations": 25,
              "donationsReceived": 67
          },
          {
              "name": "suman",
              "role": "member",
              "league": "Master League III",
              "trophies": 2615,
              "donations": 192,
              "donationsReceived": 233
          },
          {
              "name": "Atok",
              "role": "member",
              "league": "Master League III",
              "trophies": 2613,
              "donations": 212,
              "donationsReceived": 0
          },
          {
              "name": "upyggid",
              "role": "member",
              "league": "Master League III",
              "trophies": 2601,
              "donations": 326,
              "donationsReceived": 1439
          },
          {
              "name": "KRH2020",
              "role": "admin",
              "league": "Master League III",
              "trophies": 2591,
              "donations": 64,
              "donationsReceived": 247
          },
          {
              "name": "Warrior Ritam",
              "role": "admin",
              "league": "Master League III",
              "trophies": 2587,
              "donations": 33,
              "donationsReceived": 214
          },
          {
              "name": "karatemaster",
              "role": "member",
              "league": "Crystal League I",
              "trophies": 2547,
              "donations": 363,
              "donationsReceived": 132
          },
          {
              "name": "Matthijs12",
              "role": "member",
              "league": "Crystal League I",
              "trophies": 2535,
              "donations": 1237,
              "donationsReceived": 383
          },
          {
              "name": "Danny",
              "role": "member",
              "league": "Crystal League I",
              "trophies": 2525,
              "donations": 2,
              "donationsReceived": 66
          },
          {
              "name": "Tsunami",
              "role": "coLeader",
              "league": "Crystal League I",
              "trophies": 2393,
              "donations": 93,
              "donationsReceived": 200
          },
          {
              "name": "riise",
              "role": "member",
              "league": "Crystal League II",
              "trophies": 2351,
              "donations": 31,
              "donationsReceived": 134
          },
          {
              "name": "ABHAY K.",
              "role": "member",
              "league": "Crystal League III",
              "trophies": 2101,
              "donations": 78,
              "donationsReceived": 295
          },
          {
              "name": "ChaosBacca",
              "role": "member",
              "league": "Crystal League III",
              "trophies": 2075,
              "donations": 24,
              "donationsReceived": 0
          },
          {
              "name": "tim",
              "role": "member",
              "league": "Unranked",
              "trophies": 1918,
              "donations": 0,
              "donationsReceived": 0
          },
          {
              "name": "DarkFDGOD",
              "role": "admin",
              "league": "Gold League I",
              "trophies": 1891,
              "donations": 226,
              "donationsReceived": 67
          },
          {
              "name": "Digler",
              "role": "coLeader",
              "league": "Gold League I",
              "trophies": 1835,
              "donations": 3215,
              "donationsReceived": 1887
          },
          {
              "name": "WildRage",
              "role": "member",
              "league": "Gold League I",
              "trophies": 1775,
              "donations": 3,
              "donationsReceived": 25
          },
          {
              "name": "Spencer",
              "role": "member",
              "league": "Gold League I",
              "trophies": 1774,
              "donations": 111,
              "donationsReceived": 30
          },
          {
              "name": "TheGoddessMai",
              "role": "member",
              "league": "Silver League I",
              "trophies": 1335,
              "donations": 0,
              "donationsReceived": 26
          }
        ]
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.table-container {
  margin: 30px;
  width: auto;
}
.table {
  width: 100%;
}
</style>
