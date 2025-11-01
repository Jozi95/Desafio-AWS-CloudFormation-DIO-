# 📝 Insights e Anotações – Desafio CloudFormation

## 1. Planejamento da Infraestrutura
- Decidi criar um **bucket S3** e uma **instância EC2** como recursos principais.
- Defini nomes claros para cada recurso, pensando em evitar conflitos com outros stacks.
- Escolhi **t2.micro** para EC2 para manter dentro da camada gratuita da AWS.

---

## 2. Estrutura do Template
- Separei cada recurso com indentação correta em YAML.
- Usei a tag **Name** para identificar recursos facilmente no console.
- Incluí comentários explicativos no template para cada recurso.

---

## 3. Comandos e Validação
- Usei `aws cloudformation validate-template` para validar antes da criação.
- Aprendi que mesmo erros pequenos no YAML podem impedir a execução do stack.
- O comando `aws cloudformation describe-stacks` foi útil para acompanhar o progresso da criação.

---

## 4. Dificuldades Encontradas
- **Chave SSH (KeyName)**: tive que criar uma key pair na região correta.
- **ID da AMI**: cada região possui AMIs diferentes; foi necessário conferir a AMI correta para Amazon Linux 2.
- **Erros de indentação**: YAML exige atenção total à estrutura.

---

## 5. Aprendizados Importantes
- **CloudFormation** permite criar, atualizar e destruir recursos de forma padronizada.
- Automatizar infraestrutura reduz riscos de erro humano e aumenta produtividade.
- Documentar cada passo facilita o entendimento e manutenção futura.
- Versionar templates no **GitHub** é essencial para controle e colaboração.

---

## 6. Próximos Passos
- Experimentar adicionar mais recursos, como **VPC, Security Groups e RDS**.
- Criar **templates modulares**, separados por tipo de recurso.
- Explorar **parâmetros e outputs** do CloudFormation para maior flexibilidade.
- Estudar integração com **CI/CD** para deploy automático.

---

## 7. Reflexão Final
Esse desafio reforçou o conceito de **Infraestrutura como Código (IaC)**, mostrando na prática como a AWS facilita a criação e gestão de recursos.  
Documentar e versionar tudo no GitHub aumenta a confiabilidade e torna o aprendizado mais efetivo.

