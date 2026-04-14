---
title: "C\xF3mo entender tu factura"
article_id: 360021047619
translation_id: 360021047619
locale: es
sidebar_position: 7
created_at: '2021-04-13T06:37:58Z'
updated_at: '2025-10-10T07:52:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

Tus facturas son generadas por nuestro proveedor de facturación Stripe e incluyen los detalles de tu compra, los datos de la empresa, el número de recibo o factura y el método de pago utilizado. Obtén más información sobre cómo se muestran los cargos, créditos y ajustes en tu factura de Miro.

> **Disponible para**: Plan Starter, plan Business
> **Relevante para:** Admins, admins de facturación

## Dónde encontrar tus facturas

### Correos de facturación

En tu configuración de facturación, puedes especificar una dirección de correo electrónico para recibir toda la comunicación relacionada con facturación. Stripe creará tu recibo y factura, y los enviará a tu dirección de correo electrónico de facturación desde:

```
receipts+**********@stripe.com
invoice+statements+***************@stripe.com
```

### Configuración de facturación de Miro

Puedes encontrar tus facturas de Stripe en la configuración de facturación de Miro. Obtén información sobre [cómo encontrar y descargar una factura](01-how-to-find-and-download-an-invoice.md).

## Comprender los cargos en tu factura

Tu próxima factura mostrará cualquier cambio como agregar o eliminar licencias, o cambiar tu plan. Cuando cambies de plan, recibirás una nueva factura llamada **Renovación** en tu configuración de facturación.

### Cómo aparecen los cargos prorrateados

Siempre que hagas cambios en tus licencias, ya sea añadiéndolas o eliminándolas, tu factura incluirá dos líneas adicionales para mayor claridad: **Tiempo restante** y **Tiempo no utilizado**.

- **Tiempo restante** refleja el número actualizado de licencias después de tus cambios recientes.
- **Tiempo no utilizado** muestra la cantidad de licencias que tenías antes de realizar cualquier cambio.

Si ves cargos que no entiendes, consulta nuestra guía sobre [gestión de licencias adicionales](../../administration/user-management/04-manage-extra-licenses.md).

#### Agregar licencias

Si añades más licencias de las que incluye tu plan actual, se te cobrará un monto prorrateado por cada licencia adicional hasta el final de tu período de facturación. Por ejemplo, si agregaste una licencia el 23 de marzo de 2021, verás un cargo prorrateado por ella.

![charge_for_an_additional_license.jpg](../../../../../../docs/plans-billing/billing-and-payments/images/21017592958994_charge%20for%20an%20additional%20license.jpg)*El cargo prorrateado por añadir una licencia*

#### Eliminación de licencias

Si has programado la eliminación de una licencia, entrará en vigor en tu fecha de renovación. Para más información, consulta [la facturación mensual y anual de Miro](04-miro-billing.md).

#### Cambios en tu plan

Cambiar tu plan de Miro o pasar de una suscripción mensual a una anual ajusta el costo en tu próxima factura. Cualquier crédito por tiempo no utilizado en tu plan anterior se aplicará a la nueva factura. Por ejemplo, el crédito de una suscripción mensual no utilizada se puede usar en tu nueva suscripción anual. suscripción.

![amount_for_switch_to_yearly.jpg](../../../../../../docs/plans-billing/billing-and-payments/images/21017605966098_amount%20for%20switch%20to%20yearly.jpg)
*Crédito por tiempo no utilizado en una suscripción mensual aplicado a la nueva suscripción anual*

## Preguntas frecuentes

**¿Cuál es la dirección comercial de Miro?**

Puedes encontrar nuestra dirección comercial en todas las facturas y recibos de Miro:
201 Spear Street Suite 1100 San Francisco, CA, EE. UU. 94105

**¿El número de IVA de Miro se mostrará en mis facturas?**

Miro es una empresa con sede en Estados Unidos y está registrada ante el IVA de la UE a través del esquema de ventanilla única en los Países Bajos. Miro no tiene un número de ID de IVA oficial ni requisitos de facturación específicos.
