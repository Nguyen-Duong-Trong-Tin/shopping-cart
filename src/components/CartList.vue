<template>
  <table class="table">
    <thead>
      <tr>
        <th>Order number</th>
        <th>Name</th>
        <th>Unit price</th>
        <th>Stock</th>
        <th>Quantity</th>
        <th>Total price</th>
        <th>Actions</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td scope="row">1</td>
        <td>Mac book pro m1</td>
        <td>20000</td>
        <td>37</td>
        <td>
          <input type="number" min="1" max="37" value="1" />
        </td>
        <td>
          40000
        </td>
        <td>
          <button class="btn btn-danger">
            Delete
          </button>
        </td>
      </tr>
    </tbody>
  </table>
</template>

<script>
export default {
  name: "CartList"
}
</script>

<style scoped></style>