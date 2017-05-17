# magento-redsys

Versión mejorada y con corrección de errores del módulo oficial de Redsys para Magento 1.

## Mejoras

* Permite configurar el estado de los nuevos pedidos una vez pagados

## Errores corregidos

* Los pedidos se generan en estado `pending` en vez de en estado `processing` y luego cambiar a pending.
* Si un usuario pulsaba el botón de atrás de su navegador después de pagar el pedido volvía de `processing` a `pending`, es decir, se anulaba el pago de cara a Magento.
* Si el pedido estaba cancelado, por la razón que sea, y llega la notificación del pago se anota como comentario pero no se modifica el estado del pedido.
* Cuando un pedido se pagaba con importe incorrecto se generaba la factura igualmente.
* Al pagar un pedido no se borraba el carrito.
* Sólo se permiten cancelar pedidos pending por parte de redsys
* Permitimos la devolución parcial de pedidos pagados con redsys.
