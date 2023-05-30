<!DOCTYPE html>
<html>
<head>
  <title>Tabela com Numeração Automática</title>
  <script>
    window.addEventListener('DOMContentLoaded', function() {
      var table = document.getElementById('myTable');
      var tableRows = table.getElementsByTagName('tr');

      for (var i = 0; i < tableRows.length; i++) {
        var tableHeaderCell = document.createElement('th');
        tableHeaderCell.textContent = 'Página ' + (i + 1);
        tableRows[i].insertBefore(tableHeaderCell, tableRows[i].firstChild);
      }
    });
  </script>
</head>
<body>
  <table id="myTable">
    <thead>
      <tr>
        <th></th>
        <th>Coluna 1</th>
        <th>Coluna 2</th>
        <!-- Adicione mais colunas aqui, se necessário -->
      </tr>
    </thead>
    <tbody>
      <!-- Adicione as linhas da tabela aqui -->
      <tr>
        <td></td>
        <td>Dados 1</td>
        <td>Dados 2</td>
        <!-- Adicione mais células aqui, se necessário -->
      </tr>
    </tbody>
  </table>
</body>
</html>
