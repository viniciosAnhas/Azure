<div align="center">
  <div>
    <img height = "150" width = "150" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/azure/azure-original-wordmark.svg" />
  </div>
</div>

<h1>Azure Subscription</h1>

<p style="text-align: justify;">Azure Subscription é uma entidade lógica que agrupa recursos do Azure e define como você consome e paga pelos serviços. Ela também estabelece limites administrativos e de acesso.</p>

<p style="text-align: justify;">Principais funções da Assinatura:</p>

<ol>
  <li style="text-align: justify;">Cobrança (Billing)</li>
  <ul>
    <li style="text-align: justify;">Cada assinatura tem seu próprio modelo de cobrança e fatura.</li>
    <li style="text-align: justify;">Ideal para separar contas por projetos, departamentos ou ambientes (ex: produção, teste, desenvolvimento).</li>
  </ul>
  <li style="text-align: justify;">Gerenciamento de Recursos</li>
  <ul>
    <li style="text-align: justify;">Os recursos criados dentro de uma assinatura são isolados logicamente dos de outras assinaturas.</li>
    <li style="text-align: justify;">Cada assinatura possui seus próprios limites de capacidade (quotas).</li>
  </ul>
  <li style="text-align: justify;">Controle de Acesso</li>
  <ul>
    <li style="text-align: justify;">Permissões e políticas podem ser aplicadas no nível da assinatura usando o Azure RBAC (Role-Based Access Control).</li>
  </ul>
</ol>

<p style="text-align: justify;">Estrutura Hierárquica no Azure:</p>

```yaml
Azure Tenant (Diretório do Azure AD)
└── Management Group (opcional)
    └── Subscription (Assinatura)
        └── Resource Groups
            └── Recursos individuais
```

<p style="text-align: justify;">Exemplos de uso de múltiplas assinaturas:</p>

<ul>

  <li style="text-align: justify;">Separar ambientes: produção em uma assinatura, desenvolvimento em outra.</li>

  <li style="text-align: justify;">Separar clientes: empresas que fornecem serviços para outros clientes (MSPs).</li>

  <li style="text-align: justify;">Separar departamentos: marketing, finanças e TI com assinaturas próprias.</li>

  <li style="text-align: justify;">Aplicar diferentes políticas de governança e segurança.</li>

</ul>

<p style="text-align: justify;">Importante:</p>

<ul>

  <li style="text-align: justify;">Cada conta do Azure pode ter uma ou mais assinaturas.</li>

  <li style="text-align: justify;">É possível mover recursos entre assinaturas, com certas restrições.</li>

  <li style="text-align: justify;">Assinaturas podem ser agrupadas sob Management Groups, facilitando governança em ambientes grandes.</li>

</ul>