<template>
  <div class="">
    <header class="m-5">
      <h1 class="text-xl">Bóveda de timbrado</h1>
      <div class="mt-3 flex">
        <p>Consultado de timbrado de facturas de:</p>
        <p>EKU9003173C9</p>
      </div>
    </header>
    <form action="" class="grid grid-cols-5 gap-6 m-5">
      <input type="date" class="shadow-md" />
      <input type="text" placeholder="RFC Receptor" class="shadow-md" />
      <input type="text" placeholder="Serie" class="shadow-md" />
      <input type="text" placeholder="Folio" class="shadow-md" />
      <input type="text" placeholder="Tipo de comprobante" class="shadow-md" />
      <input type="text" placeholder="Monto Mínimo" class="shadow-md" />
      <input type="text" placeholder="Monto Máximo" class="shadow-md" />
      <Radio option1="3.3" option2="4.4"></Radio>
      <Radio option1="Emitidas" option2="Canceladas"></Radio>
      <button class="bg-blue-700 text-white rounded-xl">
        <i class="fa-solid fa-magnifying-glass"></i> Buscar
      </button>
    </form>
    <div class="flex justify-center">
      <table class="table-auto text-left w-full m-6">
        <thead>
          <tr>
            <th><input type="checkbox" /></th>
            <th>Ver</th>
            <th>Guardar Plantilla</th>
            <th>RFC Receptor</th>
            <th>Nombre Receptor</th>
            <th>Serie</th>
            <th>Folio</th>
            <th>Fecha</th>
            <th>Subtotal</th>
            <th>Total</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><input type="checkbox" /></td>
            <td><i class="fa-solid fa-eye"></i></td>
            <td><i class="fa-solid fa-box-archive"></i></td>
            <td>XIA123456</td>
            <td>XENON INDUSTRIAL ARTICLES</td>
            <td>ABC</td>
            <td>123</td>
            <td>2022-08-26T11:11:29</td>
            <td>$0.0</td>
            <td>$0.0</td>
          </tr>
          <tr>
            <td><input type="checkbox" /></td>
            <td><i class="fa-solid fa-eye"></i></td>
            <td><i class="fa-solid fa-box-archive"></i></td>
            <td>XIA123456</td>
            <td>XENON INDUSTRIAL ARTICLES</td>
            <td>ABC</td>
            <td>123</td>
            <td>2022-08-26T11:11:29</td>
            <td>$0.0</td>
            <td>$0.0</td>
          </tr>
          <tr>
            <td><input type="checkbox" /></td>
            <td><i class="fa-solid fa-eye"></i></td>
            <td><i class="fa-solid fa-box-archive"></i></td>
            <td>XIA123456</td>
            <td>XENON INDUSTRIAL ARTICLES</td>
            <td>ABC</td>
            <td>123</td>
            <td>2022-08-26T11:11:29</td>
            <td>$0.0</td>
            <td>$0.0</td>
          </tr>
          <tr>
            <td><input type="checkbox" /></td>
            <td><i class="fa-solid fa-eye"></i></td>
            <td><i class="fa-solid fa-box-archive"></i></td>
            <td>XIA123456</td>
            <td>XENON INDUSTRIAL ARTICLES</td>
            <td>ABC</td>
            <td>123</td>
            <td>2022-08-26T11:11:29</td>
            <td>$0.0</td>
            <td>$0.0</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script setup>
import Radio from "./Radio.vue";
</script>
