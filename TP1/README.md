# Les méthodes itératif 
## Introduction chapitre 1
 les solutions de l’´equation f(x) = 0  et f(α)=0, α est un zéro de f Le calcul de telle α n'est pas facile en générale analytiqument.C'est pourquoiqs, on a recours à des méthodes iteratives Pour approcher telle α.  L’id´ee g´en´erale est de contruire une suite (xn) qui converge vers

#### On se dispose de 3 m´ethodes pour contruire telle (xn), qui sont  :
* la méthode de la dichotomie (ou bissection)
* la méthode de point ﬁxe
* la méthode de Newton

## Partie Théorique
1.  __Principe de la méthode de dichotomie ( ou bisection )__ :
Considérons une fonction f continue sur un intervalle [a,b]. On suppose que f admet une et une seule racine α dans ]a, b[ et que f(a)*f(b)<0.
On note x=(a+b)/2le milieu de l'intervale [a,b]

* Si f(x) = 0, c’est la racine de f et le problème est résolu(α=x)
* Si $f(x) \neq 0$, nous regardons le signe de f(a)* f(x).
      si f(a)*f(x)<0 donc la racine se trouve dans l'intervalle [a,x]
      si f(a)*f(x)>0 donc la racine se trouve dans l'intervalle [x,b]
      
      
On recommence le processus en segmente chaque fois sur 2 l'intervalle ou quelle la racine est appartient jusqu'a avoir une valeur approcher sur l'intervalle adéquat.

2.  __Principe de la méthode de point fixe__

Le principe de cette méthode consiste à transformer l’équation f(x) = 0 en une équation équivalente g(x) = x . Le point α est alors un point fixe de g. Approcher les zéros de f revient à approcher les points fixes de g. Le choix de la fonction g est motivé par les exigences du théorème de point fixe. En effet, elle doit être contractante dans un voisinage I de α, ce qui revient à vérifier que : |g'(x)| <1 sur ce voisinage


3.  __Principe de la méthode de newton__

la méthode de newton c'est un cas particulier de méthode de point fixe  dont la fonction g(x) est bien défini a partir de l'equation de tangente .
L'idée est de remplacer la courbe représentative de la fonction par sa tangente.
On part d'un point x0 de l'intervalle de définition de f, et on considère la tangente à la courbe représentative de f en (x0,f(x0)). Soit x1 l'abscisse de l'intersection de la tangente avec l'axe des abscisses. Puisque la tangente est proche de la courbe, on peut espérer que x1 donne une meilleure estimation d'une solution de l'équation f(x)=0 que x0.

## Conclusion Générale 
> Pour comparer ces méthodes il faut tenir compte de la présence de ces différente aspect:
- Assure de la convergence
- vitesse de la convergence
- La précision 
- effcacité des calculs(ex:nombre d'opération)
### Tableau comparatif des méthodes :

| Dicotomie                 | Point fixe                      | Newton                              |
|---------------------------|---------------------------------|-------------------------------------|
| Lente                     | Rapide                          | Rapide                              |
| convergente               | convergence local ou divergence | convergence local                   |
| orde de convergence est 1 | dépend des dérivé               | ordre de convergence est au moins 2 |
