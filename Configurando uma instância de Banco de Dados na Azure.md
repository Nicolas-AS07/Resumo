# Resumo

Explica as configurações avançadas e fornece dicas de como iniciar um projeto utilizando uma máquina virtual. Mesmo quem prefere usar código deve aprender a configurar toda a VM, pois assim evita erros desnecessários e dores de cabeça futuras.

## Abaixo vai estar algumas dicas sobre microsoft azure que reuni enquanto pesquisava:

- Escolha o tamanho certo da VM:
Não adianta pegar uma VM muito poderosa (tipo série D ou E) se vai usar pouco. Comece com a B1s ou B2s (baixo custo) pra testes e dev.

- Use grupos de recursos:
Sempre crie um grupo de recursos por projeto. Isso facilita apagar tudo depois, sem deixar rastros.

- Defina regiões próximas:
Escolha a região do Azure mais próxima de você ou do seu público. Isso melhora o desempenho e reduz latência.

- Evite IPs públicos se não for usar:
Se não precisa acessar de fora, não ative IP público. Menos risco de ataque.

- Crie regras de firewall (NSG) simples e seguras:
Permita só o que precisa: RDP (porta 3389) ou SSH (porta 22), e só pro seu IP.

- Use disco gerenciado padrão no começo:
O disco SSD premium é mais rápido, mas o disco padrão (HDD) já serve bem pra testes e economiza grana.

- Ative auto shutdown:
Se esquecer a VM ligada, vai pagar. Ative o auto shutdown pra desligar ela todo dia num horário certo.

- Tags são seus amigos:
Use tags tipo: Projeto=Testes, Ambiente=Dev, Responsável=Nicolas. Ajuda a organizar e a entender depois.


## Essas são dicas básicas
