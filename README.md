# FastAPI Project on Binder

Para acessar a API FastAPI, clique no botão `Launch Binder`. Após o ambiente ser iniciado, a aplicação FastAPI estará rodando em um contêiner.

Você pode acessar a API através da URL fornecida pelo Binder. A API estará rodando em `http://<YOUR-BINDER-URL>/proxy/8080`, onde `<YOUR-BINDER-URL>` é a URL específica gerada pelo Binder para o seu projeto.

## Start command

```bash
uvicorn main:app --host 0.0.0.0 --port 8080
```

## Test

```bash
curl -X POST "http://host/generate_report/" -H "Content-Type: application/json" -d '{"text": "Paciente, sexo masculino, 45 anos, apresenta histórico de hipertensão e diabetes tipo 2. Queixa-se de dores torácicas intermitentes há duas semanas, piorando com esforço físico. Relata sensação de falta de ar e tontura. Exames realizados: ECG mostrou sinais de isquemia miocárdica, ecocardiograma revelou disfunção diastólica leve. Exames laboratoriais indicam níveis elevados de troponina. Paciente foi orientado a realizar cateterismo cardíaco para avaliação mais detalhada. Medicações prescritas: Atenolol 50mg uma vez ao dia, Metformina 850mg duas vezes ao dia. Recomenda-se acompanhamento com cardiologista e endocrinologista, além de dieta hipossódica e controle rigoroso da glicemia."}'
```
