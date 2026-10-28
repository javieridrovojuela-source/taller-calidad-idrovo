# Taller de Calidad del Software - Idrovo

Este proyecto implementa un servicio simple de transferencia bancaria con pruebas automatizadas.

## Descripción

Sistema de transferencias bancarias que valida:
- Montos positivos
- Cuentas existentes
- Saldo suficiente
- Cuentas diferentes (origen ≠ destino)

## Estructura del proyecto

```
taller_calidad_idrovo/
├── banco.py              # Servicio de transferencias
├── test_banco.py         # Pruebas unitarias
├── requirements.txt      # Dependencias
└── .github/
    └── workflows/
        └── calidad.yml   # CI/CD con GitHub Actions
```

## Instalación

```bash
python -m pip install -r requirements.txt
```

## Ejecutar pruebas

```bash
# Ejecutar todas las pruebas
python -m pytest -v

# Con cobertura de código
python -m pytest --cov=banco --cov-report=term-missing --cov-fail-under=81
```

## Cobertura actual

- **7 pruebas**: Todas pasando ✅
- **Cobertura**: 100% de líneas

## Integración Continua

Las pruebas se ejecutan automáticamente en cada push mediante GitHub Actions.
