metadata.name: Es el nombre que le das a la regla de Prometheus.

metadata.namespace: Especifica el namespace en el que deseas crear la regla.

spec.groups: Define los grupos de reglas que quieres incluir en esta definición. Puedes tener varios grupos con diferentes reglas dentro de cada uno.

spec.groups.name: Nombre del grupo de reglas. Puedes elegir el nombre que desees.

spec.groups.rules: Lista de reglas dentro del grupo.

spec.groups.rules.alert: Nombre de la alerta. Debe ser único dentro del grupo.

spec.groups.rules.expr: Expresión de consulta de Prometheus que define la condición para activar la alerta. En este ejemplo, la alerta se activará si la métrica "up" es igual a 0.

spec.groups.rules.for: Duración mínima durante la cual debe cumplirse la condición antes de que se active la alerta. En este caso, debe ser 0 durante al menos 5 minutos.

spec.groups.rules.labels: Etiquetas asociadas a la alerta. Puedes utilizar etiquetas personalizadas para clasificar y filtrar las alertas.

spec.groups.rules.annotations: Anotaciones adicionales que proporcionan información descriptiva sobre la alerta.