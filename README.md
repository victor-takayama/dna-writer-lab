# DNA Writer Lab - Landing Page

## 🚀 Deploy Rápido no Vercel

### Passo 1: Preparar o Repositório GitHub

1. Crie um novo repositório no GitHub chamado `dna-writer-lab`
2. Faça upload dos arquivos:
   - index.html
   - package.json
   - vercel.json
   - README.md

### Passo 2: Deploy no Vercel

1. Acesse [vercel.com](https://vercel.com)
2. Faça login com sua conta GitHub
3. Clique em "New Project"
4. Importe o repositório `dna-writer-lab`
5. Clique em "Deploy"
6. Pronto! Sua landing page estará online em minutos

### Passo 3: Domínio Personalizado (Opcional)

1. No painel do Vercel, vá em "Settings" > "Domains"
2. Adicione seu domínio: dnawriterlab.com.br
3. Configure os DNS conforme instruções do Vercel

## 💳 Configuração de Pagamentos

### Opção 1: Stripe (Recomendado - Internacional)

1. Crie conta em [stripe.com](https://stripe.com)
2. Configure produtos:
   - Executive: R$ 997/mês
   - Premium: R$ 1.497/mês
3. Gere links de pagamento recorrente
4. Substitua no código:
   ```javascript
   window.location.href = `SEU_LINK_STRIPE_AQUI`;
   ```

### Opção 2: PagSeguro/Mercado Pago (Nacional)

1. Crie conta empresarial
2. Configure planos recorrentes:
   - Plano Executive
   - Plano Premium
3. Gere links ou integre API
4. Substitua no código conforme documentação

### Opção 3: Hotmart/Eduzz (Mais Simples)

1. Crie produto de assinatura
2. Configure checkout transparente
3. Use links diretos no código

## 🔧 Customizações Importantes

### Alterar Cores
```css
:root {
    --primary: #0F3D4A;     /* Azul escuro */
    --secondary: #2B8B98;   /* Azul médio */
    --accent: #F5E6D3;      /* Bege */
}
```

### Alterar Preços
Busque por `R$ 997` e `R$ 1.497` no arquivo HTML

### Adicionar WhatsApp
Substitua `5511999999999` pelo seu número

### Google Analytics
Adicione antes do `</head>`:
```html
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

## 📊 Tracking de Conversão

### Facebook Pixel
```html
<!-- Facebook Pixel Code -->
<script>
!function(f,b,e,v,n,t,s)
{if(f.fbq)return;n=f.fbq=function(){n.callMethod?
n.callMethod.apply(n,arguments):n.queue.push(arguments)};
if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version='2.0';
n.queue=[];t=b.createElement(e);t.async=!0;
t.src=v;s=b.getElementsByTagName(e)[0];
s.parentNode.insertBefore(t,s)}(window,document,'script',
'https://connect.facebook.net/en_US/fbevents.js');
fbq('init', 'YOUR_PIXEL_ID');
fbq('track', 'PageView');
</script>
```

### Google Ads Conversion
```html
<!-- Event snippet for Purchase conversion page -->
<script>
  gtag('event', 'conversion', {
      'send_to': 'AW-XXXXXXXXX/XXXXXXXXXXXXXXXXXXX',
      'value': 997.0,
      'currency': 'BRL',
      'transaction_id': ''
  });
</script>
```

## 🎨 Elementos de Conversão

A landing page já inclui:

- ✅ Countdown timer (urgência)
- ✅ Depoimentos sociais
- ✅ FAQ para objeções
- ✅ Garantia de 7 dias
- ✅ Escassez (10 vagas/mês)
- ✅ Relatórios transparentes
- ✅ Mobile responsive
- ✅ Animações suaves
- ✅ CTAs estratégicos

## 📈 Otimizações Pós-Lançamento

### A/B Testing Sugerido
1. Teste preços: R$ 797 vs R$ 997
2. Teste headlines diferentes
3. Teste com/sem countdown
4. Teste cores dos botões

### Métricas para Acompanhar
- Taxa de conversão (meta: 2-3%)
- Tempo na página (meta: 2+ minutos)
- Taxa de rejeição (meta: <40%)
- Scroll depth (meta: 80%+)

## 🚨 Importante

### Compliance Legal
- Adicione Termos de Uso
- Adicione Política de Privacidade
- Configure LGPD compliance
- Adicione aviso de cookies

### Suporte ao Cliente
- Configure email automático pós-compra
- Crie FAQ expandido
- Configure chat (Intercom/Crisp)
- Prepare onboarding automático

## 💡 Dicas de Lançamento

1. **Soft Launch**: Teste com 5 pessoas primeiro
2. **Coleta Feedback**: Ajuste baseado em objeções reais
3. **Prova Social**: Adicione prints de resultados reais
4. **Remarketing**: Configure pixels antes do tráfego
5. **Email List**: Capture emails mesmo sem compra

## 📞 Suporte

Para dúvidas sobre a implementação:
- GitHub: github.com/seu-usuario/dna-writer-lab
- Email: contato@dnawriterlab.com

---

**Lembre-se**: O sucesso está em testar, medir e otimizar constantemente!