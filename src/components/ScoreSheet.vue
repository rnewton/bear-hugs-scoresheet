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
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
      </tr>

      <tr>
        <td class="category"><img src="@/assets/mustache.svg" alt="Mustaches" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
      </tr>

      <tr>
        <td class="category"><img src="@/assets/hat.svg" alt="Party Hats" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
      </tr>

      <tr>
        <td class="category"><img src="@/assets/necklace.svg" alt="Gold Chains" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
      </tr>

      <tr>
        <td class="category"><img src="@/assets/glasses.svg" alt="Sunglasses" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
      </tr>

      <tr>
        <td class="category"><img src="@/assets/bear-pair.svg" alt="Bear Pairs" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
      </tr>

      <tr>
        <td class="category"><img src="@/assets/false-bear-set.svg" alt="False Bear Sets" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
      </tr>

      <tr>
        <td class="category"><img src="@/assets/ranger.svg" alt="Rangers" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
      </tr>

      <tr>
        <td class="category">Total</td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
        <td><input type="number" min="0" /></td>
      </tr>
    </tbody>
  </table>
</template>

<script>
export default {
  name: 'ScoreSheet',
  props: {
    msg: String
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

.fill {
  background-color: #fafafa;
}

.category {
  font-size: 2em;
  vertical-align: middle;
}
</style>
