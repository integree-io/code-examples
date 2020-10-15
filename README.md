**[INTEGREE.IO](https://integree.io/)**
========

IMPORTAR API.JS:
---------------

* Importar api.js no header da página:
~~~js script
<script src="https://vc.integree.io/api.js"></script>
~~~

PARA CRIAR WIDGET:
-------------

* Adicionar no final da pagina:
~~~js script
<script>
    const api = new ConferenciaCorpMeet('PUBLIC-KEY'); // SETAR CHAVE PÚBLICA DA API
    const widget = api.createWidget();
    widget.start();
</script>
~~~

PARA CRIAR CONFERÊNCIA (SEM WIDGET):
-------------------------------

* Adicionar no final da pagina:
~~~js script
<script>
    const api = new ConferenciaCorpMeet('PUBLIC-KEY'); // SETAR CHAVE PÚBLICA DA API
    const room = api.newRoom('NOME DA MINHA CONFERÊNCIA', {});
    room.start();
</script>
~~~