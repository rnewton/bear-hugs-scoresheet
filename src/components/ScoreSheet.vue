<template>
  <table class="table is-striped is-fullwidth">
    <thead>
      <tr>
        <th class="fill" />
        <th><input type="text" placeholder="Name" /></th>
        <th><input type="text" placeholder="Name" /></th>
        <th><input type="text" placeholder="Name" /></th>
        <th><input type="text" placeholder="Name" /></th>
        <th><input type="text" placeholder="Name" /></th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td class="category"><img src="@/assets/bare-bear-points.svg" alt="Bare Bear Points" /></td>
        <td><input type="number" min="0" v-model="p1bare" /></td>
        <td><input type="number" min="0" v-model="p2bare" /></td>
        <td><input type="number" min="0" v-model="p3bare" /></td>
        <td><input type="number" min="0" v-model="p4bare" /></td>
        <td><input type="number" min="0" v-model="p5bare" /></td>
      </tr>

      <tr>
        <td class="category"><img src="@/assets/mustache.svg" alt="Costumes" /></td>
        <td><input type="number" min="0" step="4" v-model="p1costume" /></td>
        <td><input type="number" min="0" step="4" v-model="p2costume" /></td>
        <td><input type="number" min="0" step="4" v-model="p3costume" /></td>
        <td><input type="number" min="0" step="4" v-model="p4costume" /></td>
        <td><input type="number" min="0" step="4" v-model="p5costume" /></td>
      </tr>

      <tr>
        <td class="category"><img src="@/assets/bear-pair.svg" alt="Bear Pairs" /></td>
        <td><input type="number" min="0" step="2" v-model="p1pair" /></td>
        <td><input type="number" min="0" step="2" v-model="p2pair" /></td>
        <td><input type="number" min="0" step="2" v-model="p3pair" /></td>
        <td><input type="number" min="0" step="2" v-model="p4pair" /></td>
        <td><input type="number" min="0" step="2" v-model="p5pair" /></td>
      </tr>

      <tr>
        <td class="category"><img src="@/assets/ranger.svg" alt="Rangers" /></td>
        <td><input type="number" min="0" step="12" v-model="p1ranger" /></td>
        <td><input type="number" min="0" step="12" v-model="p2ranger" /></td>
        <td><input type="number" min="0" step="12" v-model="p3ranger" /></td>
        <td><input type="number" min="0" step="12" v-model="p4ranger" /></td>
        <td><input type="number" min="0" step="12" v-model="p5ranger" /></td>
      </tr>

      <tr>
        <td class="category">Total</td>
        <td class="total">{{ p1total }}</td>
        <td class="total">{{ p2total }}</td>
        <td class="total">{{ p3total }}</td>
        <td class="total">{{ p4total }}</td>
        <td class="total">{{ p5total }}</td>
      </tr>
    </tbody>
  </table>
</template>

<script>
export default {
  name: 'ScoreSheet',
  props: {
    msg: String
  },
  data() {
    return {
      p1bare: 0,
      p1costume: 0,
      p1pair: 0,
      p1ranger: 0,

      p2bare: 0,
      p2costume: 0,
      p2pair: 0,
      p2ranger: 0,

      p3bare: 0,
      p3costume: 0,
      p3pair: 0,
      p3ranger: 0,

      p4bare: 0,
      p4costume: 0,
      p4pair: 0,
      p4ranger: 0,

      p5bare: 0,
      p5costume: 0,
      p5pair: 0,
      p5ranger: 0,
    }
  },
  computed: {
    p1total: function() {
      return Number(this.p1bare) + Number(this.p1costume) + Number(this.p1pair) + Number(this.p1ranger)
    },
    p2total: function() {
      return Number(this.p2bare) + Number(this.p2costume) + Number(this.p2pair) + Number(this.p2ranger)
    },
    p3total: function() {
      return Number(this.p3bare) + Number(this.p3costume) + Number(this.p3pair) + Number(this.p3ranger)
    },
    p4total: function() {
      return Number(this.p4bare) + Number(this.p4costume) + Number(this.p4pair) + Number(this.p4ranger)
    },
    p5total: function() {
      return Number(this.p5bare) + Number(this.p5costume) + Number(this.p5pair) + Number(this.p5ranger)
    }
  }
}
</script>

<style scoped lang="scss">
th, td {
  height: 3em;
  table-layout: fixed;
  padding: 0;
  vertical-align: middle;

  &:first-child {
    padding: 0 20px;
  }
  &:not(:first-child) {
    border-left: 2px solid #aaa;
  }
}

input {
  font-family: 'Luckiest Guy', cursive;
  width: 100%;
  height: 100%;
  box-sizing: border-box;
  text-align: center;
  font-size: 2.5em;
  background-color: unset;
  border: none;
}

input[type=number]::-webkit-inner-spin-button, 
input[type=number]::-webkit-outer-spin-button {  
   opacity: 1;
   transform: scale(2);
}

.fill {
  background-color: #fafafa;
}

.category {
  font-size: 2em;
  vertical-align: middle;
}
.total {
  font-size: 2.8em;
  vertical-align: middle;
  text-align: center;
}
</style>
