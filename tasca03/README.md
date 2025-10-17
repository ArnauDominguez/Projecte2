# T03: Seguretat Lògica: recuperant accés a sistemes

## 1. Descripció de la situació

Després de la primera feina exitosa, arriba un **encàrrec urgent** que requereix una solució ràpida.

Com a fase prèvia, rebreu una **formació sobre seguretat lògica** per adquirir els coneixements necessaris per afrontar la tasca.

Un client ha contactat amb la consultora **EverPia** perquè té un **problema amb un portàtil que utilitzava un directiu**. L’equip utilitza **Zorin OS (Linux amb entorn gràfic)** i el directiu **ha oblidat la contrasenya d’accés**.  
A l’ordinador hi ha **documentació molt important** que cal recuperar.

Per seguretat, **el disc de l’equip s’ha clonat** en un **disc virtual**, de manera que la intervenció es farà sobre aquest **entorn virtualitzat** per evitar danys a l’equip original.

---

## 2. Objectiu de la tasca

1. **Crear una màquina virtual** i **connectar-hi el disc virtual** proporcionat.  
2. **Accedir al sistema** per descobrir **quin usuari existeix**.  
3. **Canviar la contrasenya** d’aquest usuari per poder accedir al sistema.  
4. **Verificar** que el nou accés funciona correctament.  
5. Investigar com **fortificar el sistema** per evitar que aquest procediment pugui repetir-se fàcilment.  
6. **Protegir el GRUB amb contrasenya** per evitar canvis o recuperacions no autoritzades.  
7. **Documentar tot el procés** amb **captures de pantalla i explicacions**.

---

## 3. Procediment

### 3.1 Vulnerar l’accés al GRUB

1. Inicia la màquina virtual amb Zorin OS.  
2. A la pantalla del **GRUB**, prem `e` per **editar les opcions d’arrencada**.  
3. A la línia del kernel (la que comença amb `linux`), afegeix al final:

4. Prem `Ctrl + X` per iniciar el sistema amb aquests paràmetres.  
5. El sistema arrencarà directament en una **sessió de shell com a root**.

A l'arxiu [solucio.md](solucio.md) hi ha solució descrita.

[Tornar pàgina projecte](../README.md)
