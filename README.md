##Práctica az function

Para la implementación de la AZ function fue necesario la instalación de herramientas como
terraform  y azure CLI. Con esta última se puede obtener la suscripción necesaria para la 
creación de la infraestructura. Fue necesario añadir en el provider de azurerm el subscription_id
ya que en esta nueva versión es neserio la identificación de la misma.

Luego, para evitar que Terraform solicitara el valor de name_function por consola, definí un valor por defecto en el archivo terraform.tfvars, donde se especifica lo necesario para que 
terraform pueda realizar la lectura de lar vars y asignar su valor.

```
name_function = "miknsteven"
location      = "West Europe"

```

