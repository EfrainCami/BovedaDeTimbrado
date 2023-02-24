<template>
  <div class="">
    <header class="m-5">
      <h1 class="text-xl">Bóveda de timbrado</h1>
      <div class="flex mt-3">
        <p>Consultado de timbrado de facturas de:</p>
        <p>EKU9003173C9</p>
      </div>
    </header>
    <form action="" class="grid grid-cols-5 gap-6 m-5">
      <input type="date" class="shadow-md"/>
      <input type="text" placeholder="RFC Receptor" class="shadow-md" />
      <input type="text" placeholder="Serie" class="shadow-md" />
      <input type="text" placeholder="Folio" class="shadow-md" />
      <select name="documents" class="shadow-md">
        <option value="Doc1">Tipo de documento</option>
        <option value="Doc1">Volvo</option>
        <option value="Doc2">Saab</option>
        <option value="Doc3">Mercedes</option>
        <option value="Doc4">Audi</option>
      </select>
      <input type="text" placeholder="Monto Mínimo" class="shadow-md" />
      <input type="text" placeholder="Monto Máximo" class="shadow-md" />
      <div class="flex justify-center">
        <Radio option1="3.3" option2="4.4"></Radio>
      </div>
      <div class="flex justify-center">
        <Radio option1="Emitidas" option2="Canceladas"></Radio>
      </div>
      <div class="flex justify-center">
        <button class="w-44 rounded-xl bg-blue-800 text-white">
          <i class="fa-solid fa-magnifying-glass"></i> Buscar
        </button>
      </div>

    </form>
    <div class="flex justify-end m-2">
      <p class="w-36 p-2 rounded-full bg-neutral-600 text-white">Total: 10 registros</p>
    </div>
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
          <tr class="hover:shadow-md">
            <td><input type="checkbox" /></td>
            <td><i class="fa-solid fa-eye cursor-pointer"></i></td>
            <td><i class="fa-solid fa-box-archive cursor-pointer"></i></td>
            <td>XIA123456</td>
            <td>XENON INDUSTRIAL ARTICLES</td>
            <td>ABC</td>
            <td>123</td>
            <td>2022-08-26T11:11:29</td>
            <td>$0.0</td>
            <td>$0.0</td>
          </tr>
          <tr class="hover:shadow-md">
            <td><input type="checkbox" /></td>
            <td><i class="fa-solid fa-eye cursor-pointer"></i></td>
            <td><i class="fa-solid fa-box-archive cursor-pointer"></i></td>
            <td>XIA123456</td>
            <td>XENON INDUSTRIAL ARTICLES</td>
            <td>ABC</td>
            <td>123</td>
            <td>2022-08-26T11:11:29</td>
            <td>$0.0</td>
            <td>$0.0</td>
          </tr>
          <tr class="hover:shadow-md">
            <td><input type="checkbox" /></td>
            <td><i class="fa-solid fa-eye cursor-pointer"></i></td>
            <td><i class="fa-solid fa-box-archive cursor-pointer"></i></td>
            <td>XIA123456</td>
            <td>XENON INDUSTRIAL ARTICLES</td>
            <td>ABC</td>
            <td>123</td>
            <td>2022-08-26T11:11:29</td>
            <td>$0.0</td>
            <td>$0.0</td>
          </tr>
          <tr class="hover:shadow-md">
            <td><input type="checkbox" /></td>
            <td><i class="fa-solid fa-eye cursor-pointer"></i></td>
            <td><i class="fa-solid fa-box-archive cursor-pointer"></i></td>
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
    <div class="flex justify-center">
      <button class="w-10 p-2 rounded-full text-white bg-blue-800">1</button>
    </div>
  </div>
</template>

<script setup>
import Radio from "./Radio.vue";
</script>
