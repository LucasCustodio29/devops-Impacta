# devops-Impacta
# Apache HTTP server 2.2.34
Autn / Authz:
Os módulos de autenticação e autorização agrupados foram refatados. O novo mod_authn_aliasmódulo pode simplificar bastante certas configurações de autenticação. 
Cache:
mod_cache, mod_disk_cacheE mod_mem_cachesofreram muitas mudanças, e agora são considerados de qualidade de produção. htcacheclean Foi introduzido para limpar mod_disk_cache configurações.
Configuração:
O layout de configuração padrão foi simplificado e modularizado. Os trechos de configuração que podem ser usados ​​para habilitar recursos comumente usados agora são empacotados com o Apache e podem ser adicionados facilmente à configuração do servidor principal.
Parada graciosa:
O prefork, workere event MPM agora permitem httpd desligar graciosamente através do graceful-stop sinal. A GracefulShutdownTimeoutdiretiva foi adicionada para especificar um tempo limite opcional, após o qual httpdterminará independentemente do status de qualquer solicitação que esteja sendo atendida.
Proxying:
O novo mod_proxy_balancermódulo fornece serviços de balanceamento de carga para mod_proxy. O novo mod_proxy_ajpmódulo adiciona suporte para o Apache JServ Protocol version 1.3usado pelo Apache Tomcat .
Biblioteca de expressões regulares atualizada
A versão 5.0 da Biblioteca de expressões regulares compatíveis com Perl (PCRE) está agora incluída. httpdPode ser configurado para usar a instalação do sistema do PCRE passando a --with-pcrebandeira para configurar.

# Apache HTTP Server 2.4.27
MPMs de carga em tempo de execução:
Múltiplos MPMs agora podem ser criados como módulos carregáveis em tempo de compilação. O MPM de escolha pode ser configurado em tempo de execução via LoadModulediretiva.
Evento MPM:
O Event MPM não é mais experimental, mas agora é totalmente suportado.
Suporte assíncrono:
Melhor suporte para leitura / gravação assíncrona para suporte de MPMs e plataformas.
Configuração LogLevel por módulo e por diretório:
O LogLevelagora pode ser configurado por módulo e por diretório. Novos níveis trace1 de trace8foram adicionados acima do debugnível de log.
Seções de configuração por solicitação:
<If>, <ElseIf>E as <Else> seções podem ser usadas para configurar a configuração com base em critérios por solicitação.
Analisador de expressão de propósito geral:
Um novo analisador de expressão permite especificar condições complexas usando uma sintaxe comum em directivas como SetEnvIfExpr, RewriteCond, Header, <If>, e outros.


#	NGINX
nginx-1.13.4
O ngx_http_mirror_modulemódulo (1.13.4) implementa o espelhamento de uma solicitação original criando subsequências de espelho de fundo. O resultado dos subcontratados de espelho é ignorado.
nginx-1.13.3
foram lançadas com uma correção para o estouro de números inteiros na vulnerabilidade do filtro de alcance.

#WordPress
4.6	Pepper
Agora tanto os plugins e temas podem ser instalados, atualizados ou excluídos sem recarregar a página. O painel do WordPress agora aproveita as fontes que ousuário já tem, tornando o carregamento mais rápido. O editor verifica automaticamente erros acidentais nos links criados pelo usuário e também salva no navegador tudo que é digitado, permitindo recuperação a qualquer momento.
4.7	Vaughan
Foi adicionado o tema padrão Twenty Seventeen, que trabalha com cabeçalhos em vídeo e este mesmo recurso pode ser usado em outros layouts. Agora o usuário pode personalizar enquanto instala o sistema. Na demonstração ao vivo, foi adicionado atalhos em secções do layout para facilitar a edição destes. Pode ser criado páginas diretamente enquanto se cria menus. Uma ótima ferramente que foi adicionada é o CSS customizado, onde o usuário pode adicionar seus próprios estilos diretamente no site, sem relação direta com o tema ativo. Para quem gosta de publicar arquivos PDF, agora é possível ver em miniaturas na galeria. Para quem gosta de utilizar multi idiomas, foi adicionada a possibilidade de ter vários idiomas que o usuário pode escolher ao utilizar o painel do WordPress.
