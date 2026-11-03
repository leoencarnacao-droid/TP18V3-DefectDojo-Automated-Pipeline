TP18 V3 - Automated DefectDojo Integration
Objetivo

Implementar una versión automatizada del proceso de seguridad DevSecOps utilizado en TP18 y TP18V2 mediante GitHub Actions.
Evolución del proyecto
TP18 Original

Integración manual de:

    Semgrep (SAST)
    Trivy (SCA)

Resultado:

    197 Findings centralizados en DefectDojo

TP18 V2

Integración manual ampliada:

    Semgrep
    Trivy
    Gitleaks
    Checkov

Resultado:

    251 Findings centralizados en DefectDojo

TP18 V3

Automatización mediante GitHub Actions:

    Semgrep
    Trivy
    Gitleaks
    Checkov

Generación automática de reportes JSON:

    semgrep-results.json
    trivy-report.json
    gitleaks-report.json
    checkov-report.json

Flujo DevSecOps

Git Push ↓ GitHub Actions ↓ Semgrep ↓ Trivy ↓ Gitleaks ↓ Checkov ↓ JSON Reports ↓ DefectDojo (próxima etapa)
Herramientas incluidas
Semgrep

Análisis estático de código (SAST).
Trivy

Análisis de dependencias, imágenes y CVEs.
Gitleaks

Detección de secretos y credenciales expuestas.
Checkov

Análisis de Kubernetes, Helm, YAML e Infrastructure as Code.
Próximo objetivo
Integrar automáticamente los reportes generados por GitHub Actions utilizando la API de DefectDojo para eliminar la importación manual de resultados.
