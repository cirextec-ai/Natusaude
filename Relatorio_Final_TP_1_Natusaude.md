
# Relatório Final TP_1 — Manutenção Corretiva

## 1. Breve descrição do sistema

O sistema **Natusaude** é uma aplicação destinada à gestão informatizada de processos de saúde, incluindo cadastro de pacientes, registro de atendimentos, módulos internos e funcionalidades administrativas.  
O objetivo principal é garantir agilidade, precisão e integridade das informações manipuladas pelos usuários do sistema.

**Principais funcionalidades:**
- Gestão de pacientes
- Registro de atendimentos
- Módulos administrativos
- Controle de acessos e login

**Tecnologias usadas:**
- **Backend:** Django (Python 3.11)  
- **Frontend:** HTML, CSS, JavaScript (+ Bootstrap para componentes responsivos)  
- **Banco de dados:** SQLite (desenvolvimento) / PostgreSQL (produção)  
- **Outras:** Docker, Git/GitHub, GitHub Actions (CI), SMTP para envio de e-mails

---

## 2. Lista dos bugs identificados e classificações

| # | Bug identificado | Severidade | Impacto | Prioridade |
|---|------------------|------------|---------|------------|
| 1 | Erro ao salvar atendimento: ao submeter o formulário de atendimento, ocorre exceção e o registro não é persistido. | Alta | Afeta funcionalidade crítica (registro de atendimentos) | Urgente |
| 2 | Cadastro de paciente — campo e-mail aceita valores duplicados | Média | Afeta fluxo secundário (integridade de dados) | Alta |
| 3 | Layout da tela de pacientes quebra em telas pequenas: botões sobrepostos | Baixa | Pequena falha de UI/UX | Baixa |

---

## 3. Links para issues do GitHub

1. **Bug 1** – Issue #X — substitua `X` pelo número real: `https://github.com/cirextec-ai/Natusaude/issues/X`  
2. **Bug 2** – Issue #Y — substitua `Y` pelo número real: `https://github.com/cirextec-ai/Natusaude/issues/Y`  
3. **Bug 3** – Issue #Z — substitua `Z` pelo número real: `https://github.com/cirextec-ai/Natusaude/issues/Z`

> Observação: atualize os links acima com os números reais das issues no repositório.

---

## 4. Links para commits/PRs que corrigem os bugs

| Bug | Correção | Link |
|------|-----------|-------|
| Bug 1 | PR que corrige validação e persistência de atendimentos | `https://github.com/cirextec-ai/Natusaude/commit/ID1` |
| Bug 2 | PR que adiciona restrição UNIQUE no e-mail e checagem no backend | `https://github.com/cirextec-ai/Natusaude/commit/ID2` |
| Bug 3 | PR que ajusta CSS responsivo e classes do Bootstrap | `https://github.com/cirextec-ai/Natusaude/commit/ID3` |

> Substitua `ID1`, `ID2`, `ID3` pelos hashes reais dos commits ou pelos números dos PRs.

---

## 5. Evidências dos testes de validação

### ✔ Bug 1
- **Descrição do teste:** Preencher formulário de atendimento com dados válidos e submeter. Verificar a ausência de exceções no backend e a persistência do registro na lista de atendimentos.  
- **Resultado esperado:** Atendimento salvo e visível na listagem; resposta HTTP 201 (ou redirecionamento com sucesso).  
- **Resultado obtido:** (inserir após execução dos testes)  
- **Evidência:**  
  ![Evidência Bug 1](inserir_caminho_ou_link)

---

### ✔ Bug 2
- **Descrição do teste:** Tentar cadastrar dois pacientes com o mesmo e-mail. Verificar retorno de erro e bloqueio do segundo cadastro.  
- **Resultado esperado:** Validação do backend/negar duplicidade; mensagem de erro amigável no frontend.  
- **Resultado obtido:** (inserir)  
- **Evidência:**  
  ![Evidência Bug 2](inserir_caminho_ou_link)

---

### ✔ Bug 3
- **Descrição do teste:** Abrir lista de pacientes em dispositivos com largura <= 480px e verificar layout.  
- **Resultado esperado:** UI adaptada sem sobreposição; botões visíveis e funcionais.  
- **Resultado obtido:** (inserir)  
- **Evidência:**  
  ![Evidência Bug 3](inserir_caminho_ou_link)

---

## 6. Conclusão

Durante este trabalho foram identificados e corrigidos diversos bugs que afetavam o correto funcionamento do sistema **Natusaude**.  
As correções foram validadas por meio de testes específicos, garantindo maior estabilidade e confiabilidade da aplicação.

**Lições aprendidas:**
- Importância de logs detalhados para rastrear problemas.
- Necessidade de testes automatizados.
- Adoção de boas práticas de versionamento e revisão de código.

**Próximos passos:**
- Implementar testes unitários e de integração (pytest / Django test framework).
- Criar pipeline CI/CD (GitHub Actions).
- Planejar melhorias contínuas na arquitetura (separação de serviços, monitoramento).

---

## 7. Anexos

- Capturas de tela dos testes (adicionar caminhos/links abaixo):  
  - `evidencias/bug1_screenshot.png`  
  - `evidencias/bug2_screenshot.png`  
  - `evidencias/bug3_screenshot.png`

---

### Observações finais

Este relatório foi gerado automaticamente a partir do modelo fornecido. Atualize os campos marcados com **(inserir)**, `X`, `Y`, `Z`, `ID1`, `ID2`, `ID3` e os caminhos das evidências com os valores reais do seu projeto antes de entregar.

