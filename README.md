# Diccionario de Campos del Dataset

- **rating**: Calificación: Calificación de la publicación.
- **company name**: Nombre de la Empresa: Nombre de la empresa.
- **headquarters**: Sede Central: Ubicación de la sede central.
- **founded**: Fundación: Año de fundación de la empresa.
- **company_age**: Edad de la Empresa: Edad de la empresa.
- **type of ownership**: Tipo de Propiedad: Describe el tipo de empresa (sin fines de lucro, público, privado, etc.).
- **industry**: Industria: Industria en la que trabaja la empresa.
- **sector**: Sector: Sector al que pertenece la empresa.
- **revenue**: Ingresos: Ingresos totales de la empresa.
- **competitors**: Competidores: Competidores de la empresa.
- **min_salary**: Salario Mínimo: Salario mínimo para el puesto.
- **max_salary**: Salario Máximo: Salario máximo para el puesto.
- **avg_salary**: Salario Promedio: Salario promedio para el puesto.
- **job_state**: Estado Laboral: Estado donde se encuentra el puesto de trabajo.
- **same_state**: Mismo Estado: ¿El puesto de trabajo está en el mismo estado que la sede central? (Booleano).
- **job_title**: Título del Trabajo: Título del puesto de trabajo.
- **job_level**: Nivel del Trabajo: Nivel del puesto de trabajo.
- **python**: Python: ¿Se requieren habilidades en Python? (Booleano).
- **excel**: Excel: ¿Se requieren habilidades en Excel? (Booleano).
- **sql**: SQL: ¿Se requieren habilidades en SQL? (Booleano).
- **tableau**: Tableau: ¿Se requieren habilidades en Tableau? (Booleano).
- **aws**: AWS: ¿Se requieren habilidades en AWS? (Booleano).
- **spark**: Spark: ¿Se requieren habilidades en Spark? (Booleano).
- **hadoop**: Hadoop: ¿Se requieren habilidades en Hadoop? (Booleano).
- **azure**: Azure: ¿Se requieren habilidades en Azure? (Booleano).
- **segment**: Segmento: Tamaño de la empresa basado en el número de empleados.
  - Micro: 1-10
  - Small: 11-50
  - Middle: 51-1000
  - Corporate: > 1000

Aquellos valores que son nulos se encuentran reprentados por la cadena de texto "NA".
```python
categorical_cols = ['company name','headquarters','type of ownership', 'industry', 'sector', 'revenue', 'competitors',
                'job_state', 'same_state',
                'job_title', 'job_level','segment']
cantidad_na = (df[categorical_cols] == 'NA').sum()
```
Este diccionario proporciona descripciones para cada uno de los campos del conjunto de datos.
