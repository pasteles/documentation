# Git
## Regla de oro

Nunca hacer un `rebase` de unos commit ya compartidos, es decir, una vez que se suben al Repository, se debe de evitar hacer `rebase` de esos commmit. Esto es así porque `rebase` es un comando que cambia la historia, copia todos los antiguos commit a nuevos commit. Los nuevos commit parecen como los viejos, pero son diferentes objetos en la base de datos de git. Como resultado, si se hace un rebase de commit que otros desarrolladores han compartido en el Repository, se introducen conflictos que tienen que ser resueltos de manera manual. En general no se deben de utilizar técnicas que cambien la historía sobre commit que ya han sido compartidos.