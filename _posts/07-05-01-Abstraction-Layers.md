---
isChild: true
title:   Livelli di astrazione
anchor:  databases_abstraction_layers
---

## Livelli di astrazione {#databases_abstraction_layers_title}

Molti framework forniscono il proprio livello di astrazione, che a volte è
basato su [PDO][1]. Spesso questi emulano in un sistema di database funzionalità
presenti solo in un altro, fornendoti dei metodi PHP per costruire le tue query;
in questo modo forniscono un'astrazione reale del database invece della semplice
astrazione della connessione fornita da PDO. Ovviamente, questo complica
leggermente le cose, ma se stai costruendo un'applicazione portatile che deve
funzionare con MySQL, PostgreSQL e SQLite, allora un po' di complicazione può
essere introdotta per avere del codice pulito.

Alcuni livelli di astrazione sono stati costruiti usando gli standard di
namespace [PSR-0][psr0] o [PSR-4][psr4], in modo che possano essere installati
in qualunque applicazione:

* [Aura SQL][6]
* [Doctrine2 DBAL][2]
* [Propel][7]
* [ZF2 Db][4]

[1]: http://php.net/book.pdo
[2]: http://www.doctrine-project.org/projects/dbal.html
[4]: http://packages.zendframework.com/docs/latest/manual/en/index.html#zend-db
[6]: https://github.com/auraphp/Aura.Sql
[7]: http://propelorm.org/
[psr0]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md
[psr4]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-4-autoloader.md
