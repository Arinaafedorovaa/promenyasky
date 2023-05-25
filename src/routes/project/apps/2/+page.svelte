<h1>Учет расходов</h1>

<form on:submit|preventDefault={addExpense}>
 <label for="name">Название:</label>
 <input type="text" id="name" bind:value={newName} />
 <label for="amount">Сумма:</label>
 <input type="text" id="amount" bind:value={newAmount} />
 <button type="submit">Добавить</button>
</form>

<table>
 <thead>
  <tr>
   <th>Название</th>
   <th>Сумма</th>
   <th>Действия</th>
  </tr>
 </thead>
 <tbody>
  {#each expenses as expense, i}
   <tr>
    <td><div>{expense.name}</div> </td>
    <td><div>{expense.amount}</div> </td>
    <td><button class="deleteBtn" on:click={() => deleteExpense(i)}>Удалить</button></td>
   </tr>
  {/each}
 </tbody>
</table>

<script>
 let expenses = [];

 let newName = '';
 let newAmount = '';

 function addExpense() {
  const obj = {
   name: newName,
   amount: parseInt(newAmount),
  };
  expenses.push(obj);
  expenses = expenses;
  newName = '';
  newAmount = '';
 }

 function deleteExpense(index) {
  expenses.splice(index, 1);
  expenses = expenses;
 }
</script>

<style>
 label {
  display: block;
  margin-bottom: 20px;
 }
 input[type='text'] {
  padding: 13px;
  border: 5px solid #BA55D3;
  border-radius: 5px;
  margin-right: 10px;
  width: 160px;
 }
 table {
  margin-top: 30px;
  border-collapse: collapse;
  width: 100%;
 }
 th,
 td {
  border: 3px solid #EE82EE;
  padding: 15px;
  text-align: left;
 }
 th {
  background-color: #ebd4e4;
 }
 button {
   font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  padding: 5px 10px;
  background-color: #FF69B4;
  color: rgb(248, 203, 237);
  border: none;
  border-radius: 5px;
  cursor: pointer;
 }
 .deleteBtn {
   font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    padding: 15px 20px;
    background-color: #FFC0CB;
    color: rgb(37, 85, 175);
    border: none;
    border-radius: 5px;
    cursor: pointer;
 }
 h1 {
  font-size: 30px;
  margin-bottom: 15px;
 }
</style>