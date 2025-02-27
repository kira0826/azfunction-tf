## Práctica az function

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
Se adjunta el conjunto de servicios creados en az: 

![image](https://github.com/user-attachments/assets/0609d71c-806d-4b89-954b-c65ffda432bc)

Se adjunta la respuesta de la api de la az function:

![image](https://github.com/user-attachments/assets/3f8e5f60-e48a-4b57-a82f-d4fb510bb225)

Se adjunta la información de la url de la az function:

![image](https://github.com/user-attachments/assets/0da36457-37b8-463a-ae19-a4e3132076c7)

Por último, se procede a eliminar los recursos creados con el comando ```terraform destroy```.
![image](https://github.com/user-attachments/assets/2a065a13-9506-48dc-bdfd-aca98090a5d8)

