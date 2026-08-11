class Pan {
  constructor(id, nombre, precio) {
    this.id = id;
    this.nombre = nombre;
    this.precio = precio;
  }
}

class Cliente {
  constructor(id, nombre) {
    this.id = id;
    this.nombre = nombre;
  }
}

class DetalleVenta {
  constructor(id, pan, cantidad) {
    this.id = id;
    this.pan = pan;
    this.cantidad = cantidad;
    this.subtotal = pan.precio * cantidad;
  }
}

class Venta {
  constructor(id, cliente, detalle) {
    this.id = id;
    this.cliente = cliente;
    this.detalle = detalle;
    this.total = detalle.subtotal;
  }
}
