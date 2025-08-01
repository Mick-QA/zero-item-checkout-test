# zero-item-checkout-test
Prueba manual para verificar que una app de entregas no permita enviar un pedido con 0 productos.


**ID:** QAUG-SE1  
**Nombre del caso:** Verificar que no se permita enviar un pedido con 0 productos  
**Precondiciones:** 
- Usuario con sesión iniciada  
- Cesta vacía  

**Pasos:**
1. Iniciar sesión en la aplicación.
2. Asegurarse de que la cesta esté vacía.
3. Ir directamente a la sección del carrito o intentar acceder al flujo de pago sin agregar productos.
4. Intentar confirmar un pedido sin haber agregado ningún artículo.
5. Observar el comportamiento del sistema.

**Resultado esperado:**
- El sistema debe impedir al usuario continuar con el proceso de compra si la cesta está vacía.
- Debe mostrarse un mensaje de advertencia, como: *“Agrega al menos un producto para continuar”*.
- No debe generarse ningún pedido ni número de orden.

**Resultado obtenido:**
✅ El sistema bloqueó el acceso al proceso de pago con la cesta vacía.  
✅ Se mostró el mensaje: *“Tu carrito está vacío. Agrega productos para continuar”*  
✅ No se generó número de pedido.

**Estado de la prueba:** PASADA ✅
