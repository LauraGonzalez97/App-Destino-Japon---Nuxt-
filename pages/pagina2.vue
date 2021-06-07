<template>
  <div>
    <!-- Import jQuery, FontAwesome Icons and Open Sans Font -->
    <!-- Import jQuery, FontAwesome Icons and Open Sans Font -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>

    <script
      src="https://kit.fontawesome.com/56942480bb.js"
      crossorigin="anonymous"
    ></script>

    <link

      

    
      href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600;700&display=swap"
      rel="stylesheet"
    />

    <!-- LISTA-->
    <div id="listWrapper">
      <!-- TITULO LISTA -->
      <div id="title">
        <input
          id="titleInput"
          type="text"
          placeholder="Título"
          maxlength="21"
        />
        <i class="fa fa-pencil-alt"></i>
      </div>

      <div id="separator"></div>

      <!-- TO DO -->
      <div id="itemsWrapper">
        <div class="item">
          <!-- ITEMS NUEVOS SE CREAN AQUI -->
          
          <ul
            class="list-group"
            v-for="(tarea, index) in tareas"
            v-bind:key="index"
          >
            <li class="list-group-item">
              <span class="cursor" v-on:click="actualizarTarea(tarea, index)">
                <i v-bind:class="[tarea.estado === true ? 'far fa-check-square': 'far fa-square']"></i>
                <!-- <i class="far fa-square"></i>-->
                <!-- <i class="far fa-check-square"></i>-->
                
              </span>
              <h5>
                {{ tarea.nombre }}
                </h5>
              <span class="cursor" v-on:click="eliminarTarea(index)">
                <i class="fa fa-trash"></i>
              </span>

              
            </li>
          </ul>
          
        </div>
      </div>

      <!-- Add NEW ITEM -->
      <div id="addNewItemWrapper">
        <input
          placeholder="Escribe aquí tu lista" 
          type="text"
          id="addNewItemInput"
          maxlength="30"
          v-model="nombreTarea"
          v-on:keyup.enter="agregarTarea()"
        />
        <div id="addNewItemBtn"><i class="fas fa-plus"></i></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tareas: [],
      nombreTarea: "",
    };
  },
  methods: {
    agregarTarea() {
      const tarea = {
        nombre: this.nombreTarea,
        estado: false,
      };

      this.tareas.push(tarea);
      this.nombreTarea = "";
      console.log(this.tareas);
    },
    eliminarTarea(index){
      this.tareas.splice(index, 1);
    },
    actualizarTarea(tarea, index){
      this.tareas[index].estado = !tarea.estado;
    },
  },
};
</script>

<style>

* {
  box-sizing: border-box;
  outline: none;
}

.cursor{
  cursor: pointer;
}

.list-group-item{
  display: flex;
  justify-content: space-between;
}


#listWrapper {
  background: white;
  border-radius: 9px;
  border: 1px solid #f39e9c;
  box-shadow: 0 0 30px rgba(211, 220, 248, 0.3);
  padding: 30px;
  margin-left: 30rem;
  margin-right: 30rem;
  margin-top: 3rem;
}


#title {
  position: relative;
  display: flex;
  align-items: center;
}

#titleInput {
  font-family: "Open Sans", sans-serif;
  font-size: 24px;
  font-weight: 800;
  border: 1px solid transparent;
  border-radius: 9px;
  color: #67729b;
  padding: 9px 18px;
}

#titleInput::placeholder {
  color: rgba(63, 69, 95, 0.3);
}


.fa-pencil-alt {
  font-size: 18px;
  border-radius: 50%;
  position: absolute;
  right: 24px;
  pointer-events: none;
  color: #67729b;
}


#separator {
  margin: 12px 0;
  box-shadow: 0 12px 12px #f3f6ff;
  border-top: 0;
  border-right: 0;
  border-left: 0;
  max-width: 100%;
  height: 10px;
}


#itemsWrapper {
  padding: 8px 8px;
  margin: 12px 0;
}

* {
  box-sizing: border-box;
  outline: none;
  list-style: none;
}


.item {
  width: 100%;
  font-size: 18px;
  font-family: "Open Sans", sans-serif;
  border-radius: 12px;
  border: 0;
  padding: 9px 12px;
  color: #67729b;
  position: relative;
  
}

.itemInner {
  padding: 9px 0;
  display: flex;
  align-items: center;
  font-size: 16px;
}

.itemInner p {
  margin: 0;
  pointer-events: none;
}


.fa-trash-alt {
  pointer-events: none;
  color: #67729b;
  font-size: 18px;
}

.removeItemBtn {
  position: absolute;
  right: 4px;
  background: transparent;
  border: 0;
  cursor: pointer;
  opacity: 0;
}

.fa-hand-point-right {
  color: #67729b;
  margin-right: 9px;
  font-size: 24px;
  cursor: pointer;
}


#addNewItemWrapper {
  width: 100%;
  position: relative;
  display: flex;
  align-items: center;
}

#addNewItemInput {
  width: 100%;
  font-family: "Open Sans", sans-serif;
  font-size: 16px;
  font-weight: 600;
  border: 0;
  border-radius: 9px;
  color: #67729b;
  padding: 12px 60px 12px 18px;
  background: #f3f6ff;
}

#addNewItemBtn {
  position: absolute;
  right: 0;
  padding: 0 18px;
  background: transparent;
  border: 0;
  color: #67729b;
  font-size: 18px;
}
</style>