Parc Informatique de l'EPITA
============================

Qu'est-ce que ...
-----------------

... les SM ?
    SM est l'abbréviation de *Salle Machine*. Il s'agit des salles de l'école
    où on trouve de 20 à 80 postes informatiques accessibles à tous les élèves.
    Comme le reste de l'école, ces salles sont ouvertes 24h/24.

    On en trouve à Villejuif et au Kremlin-Bicêtre : 1er étage des locaux du KB
    côté Voltaire (lab SR, Mid-lab, lab Cisco, sm14, sm15), lab Pasteur (qui
    donne sur la cour du KB), sous-sol Pasteur (sm02, sm03), 3ème étage à
    Villejuif (v301, v302, v303, v304, v306).

    Elles sont soumises à un réglement supplémentaire à celui habituel, qui est
    normalement affiché sur les murs ou sur les portes. Les quelques règles
    importantes à ne pas oublier : ne pas manger ou boire dans les salles
    machines, ne pas débrancher les machines, ne pas brancher son ordinateur
    portable, ne pas jouer avant 19h et après 8h.

... le bocal ?
    Ce sont les administrateurs système de l'école, dont le rôle est de
    maintenir le parc informatique des écoles du groupe IONIS en état de
    fonctionnement. À quelques exceptions près, les membres du bocal
    (*bocaliens*) sont des étudiants d'EPITECH travaillant au bocal à mi-temps.

    La meilleure manière d'entrer en contact avec le bocal est de faire un
    ticket de support sur l'intranet Bocal : https://intra-bocal.epitech.eu/

    S'ils vous est impossible de créer un ticket, le bocal est présent à deux
    emplacements :

    - Au Kremlin-Bicêtre, depuis la cours Pasteur montez l'escalier à droite de
      la cafétéria puis descendez l'escalier en colimaçon ;
    - Parfois à Villejuif (il n'y a pas toujours de bocaliens présents), au
      sous-sol (chercher la porte avec un logo Bocal dessus).

... le rack ?
    Le rack est un disque dur dans un boitier spécial qui permet de se brancher
    à n'importe quelle machine de l'école. Par défaut l'école vous fournit un
    boitier contenant un disque dur de 500 Go, dont environ 200 Go sont
    utilisés par le *dump* (voire en dessous) et 300 Go sont disponibles pour
    vous installer un autre OS si vous le souhaitez.

... le dump ?
    C'est le nom donné au contenu par défaut du disque du rack. Si vous n'avez
    rien modifié à votre rack, vous utilisez normalement un des 3 systèmes
    présent sur le dump du bocal. Ce dump change tous les ans - pour l'année
    scolaire 2012-2013, il est composé de 3 systèmes d'exploitations :

    - Un Windows 7 x64 avec Visual Studio et des outils de développement OCaml
    - Un Linux OpenSuse avec tous les outils nécessaires pour faire du C, du
      C++, de l'OCaml et du Java
    - Une partition *exam* utilisée pour les examens de programmation se
      passant en salle machine. Elle contient à peu près la même chose que la
      partition Linux normale. Vous ne pouvez pas l'utiliser hors des examens.
    - Une entrée *redump* dans le menu de boot qui vous permet de remettre à
      zéro votre rack à partir d'une copie du dump située sur le disque

... la feuille de passwords ?
    Elle vous est donnée en début de scolarité par le bocal. Ne la perdez
    surtout pas, et si possible gardez-en un scan quelque part (c'est moins
    facile à perdre qu'une feuille de papier).

    Comme son nom l'indique, sur cette feuille se trouvent tous les mots de
    passe dont vous aurez besoin pour accèder aux services en rapport avec
    l'école. Elle contient également vos identifiants. Notamment :

    - Le login : votre identifiant principal à l'école, composé de 6 lettres de
      votre nom de famille, un *underscore* (_) et la première lettre de votre
      prénom (quand c'est possible, sinon une autre lettre). Vous vous en
      servirez à peu près partout.
    - Le password UNIX (noté simplement `password` sur la feuille): utilisé
      pour se connecter à distance aux machines Linux de l'école, consulter vos
      mails, ou accèder à l'AFS.
    - Le password SOCKS : nécessaire pour se connecter à Netsoul et au réseau
      Wi-Fi de l'école. Nommé "SOCKS" parce qu'il servait dans le passé à se
      connecter aux proxies SOCKS de l'école, qui sont maintenant obsolètes.
    - Le password PPP : nécessaire pour se connecter à différents intranets
      (intra Bocal, intra EPITECH). Nommé "PPP" parce qu'il étant dans le passé
      utilisé pour se servir d'EPITA comme FAI via une ligne téléphonique.
    - L'UID : un numéro unique vous identifiant dans l'école. Sa seule vraie
      utilité est de s'en servir pour ouvrir les digicodes de l'école.
    - Le passcode : mot de passe numérique utilisé pour les digicodes.

    Essayez d'avoir toutes ces informations sur vous tant que vous ne les
    connaissez pas par coeur - il serait bête de se retrouver coincé dehors
    parce que vous avez oublié votre UID ou votre passcode !

... Netsoul ?
    Netsoul est un protocole réseau interne à EPITA et les écoles du groupe
    IONIS. Lorsque vous vous connectez sur une machine de l'école, vous devez
    vous connecter à Netsoul pour vous identifier et avoir accès à Internet.
    Lorsque vous êtes connectés, vous pouvez vous servir de Netsoul pour
    discuter avec d'autres étudiants. Le serveur Netsoul indique également d'où
    vous vous êtes connectés afin que n'importe qui puisse savoir où vous êtes
    dans l'école.

    Pour vous connecter à Netsoul, vous avez besoin d'un client Netsoul. Les
    plus couramments utilisés sont :

    - bNetsoul sous Windows (installé par défaut sur les racks)
    - ns_log ou jogsoul sous Linux (ns_log est installé par défaut)

    Dans le passé, Netsoul servait à plein d'autres choses : notification en
    cas de nouvel email, en cas de coup de téléphone, etc.

... l'AFS ?
    C'est le nom donné au stockage de fichiers en réseau de l'école. Tout ce
    qui est mis sur l'AFS sera disponible sur toutes les machines où vous aurez
    accès à l'AFS. Pour accèder à l'AFS, rendez-vous dans le dossier
    ``/afs/epitech.net`` sous Linux, ou ``\\AFS\epitech.net`` sous Windows.

    Vous avez par défaut un dossier personnel sur l'AFS avec un quota de 200Mo
    de stockage. Son chemin est ``/afs/epitech.net/users/all/<login>/cu`` (en
    remplaçant ``<login>`` par votre login).

... le sgoinfre ?
    Le sgoinfre est un dossier partagé sur l'AFS accessible à tout le monde en
    lecture et en écriture. Vous pouvez vous en servir pour facilement partager
    des fichiers à n'importe qui dans l'école. Attention cependant à ne pas
    vous en servir pour stocker des données importantes : le sgoinfre est vidé
    tous les jours afin que rien ne s'y accumule.

    Vous pouvez y accèder dans ``/afs/epitech.net/goinfre`` sous Linux ou
    ``\\AFS\epitech.net\goinfre`` sous Windows.

Comment ...
-----------

... verrouiller sa session ?
    Il est parfois nécessaire de s'absenter quelques minutes de son poste
    informatique (pour téléphoner, aller boire quelque chose en dehors de la
    salle machine, etc.). Si cela arrive et que vous laissez votre session
    ouverte, n'importe qui passant dans les rangs de la salle machine peut
    accèder au réseau de l'école en tant que vous, récupérer vos fichiers,
    installer des virus sur votre rack, etc. Il est donc nécessaire de
    verrouiller sa session avant de bouger de son poste, même si vous vous
    absentez pour moins d'une minute.

    Sous Windows, la fonctionnalité est disponible de base si vous avez mis un
    mot de passe correct à votre session : le raccourci clavier est Win+L.

    Sous Linux, si vous utilisez la distribution installée par défaut sur votre
    rack, vous pouvez lancer la commande ``zlock`` et cliquer sur la fenêtre
    qui apparait pour verrouiller votre session. N'oubliez surtout pas de
    cliquer sur cette fenêtre, sans quoi votre session resterait ouverte !

    Si vous n'utilisez pas la distribution Linux fournie par le bocal,
    installez au choix xtrlock ou slock, qui sont deux logiciels de
    verrouillage de session fonctionnant très bien.

... lire ses mails EPITA ?
    Sur votre feuille de password, les deux champs *email* et *remail*
    correspondent à des adresses email fournies par EPITA. L'administration va
    souvent vous envoyer des emails à cette adresse, et vous êtes censés les
    lire régulièrement.

    Chaque élève a une boite mail et plusieurs adresses qui pointent vers cette
    boite :

    - ``email@epita.fr`` (souvent ``prenom.nom@epita.fr``)
    - ``remail@epita.fr`` (souvent ``nom.prenom@epita.fr``)
    - ``login@epita.fr``
    - ``login@epitech.eu`` (pour des raisons étranges d'intra bocal qui n'envoie
      pas sur votre boite ``@epita.fr``)

    Pour lire votre boite mail, vous devez vous connecter à Outlook Live, dont
    l'URL est https://login.live.com/ . Entrez comme *Compte Microsoft*
    ``email@epita.fr`` (donc, souvent, ``prenom.nom@epita.fr``), et comme *Mot
    de passe* votre password UNIX.

... se connecter à IRC ?
    Un réseau IRC permet de discuter en temps réel avec des personnes réunies
    dans des canaux (*channels*) à thèmes. Par exemple, les étudiants d’EPITA
    ont tendance à se regrouper sur le réseau Rezosup [1]_ dans le canal de
    discussion ``#epita``. Il est possible de rejoindre des canaux IRC très
    simplement avec un client IRC tel que XChat, irssi, weechat, …

    Pour les personnes pressées, ``irssi`` est théoriquement installé sur les
    dumps : lancez ``irssi`` en ligne de commande. Dans l’interface qui
    apparaît, entrez la commande ``/connect irc.rezosup.org`` puis ``/join
    #epita``. Vous êtes prêts à discuter !

    .. [1] http://www.rezosup.org/

... signaler une machine ne fonctionnant pas ?
    Lorsque la machine sur laquelle vous travaillez a un problème, le bocal
    n'est pas *automagiquement* mis au courant. Signaler ce genre de problèmes
    vous permet de facilement contribuer à la maintenance du parc informatique
    de l'EPITA.

    Rendez vous sur l'intra bocal [2]_ et créez un ticket avec le plus
    d'informations possibles sur le problème matériel que vous avez rencontré.
    Un exemple de titre de ticket utile pourrait par exemple être le suivant :

        Souris morte sur friends (VJ salle 304, r02p10)

    Le nom de la machine est généralement inscrit sur une étiquette collée à la
    machine. `r02p10` signifie *rangée 2, poste 10*. Les rangées et numéros de
    postes sont eux aussi indiqués en bout de rangées.

    Dans le corps du ticket, mettez le plus d'informations possibles quand cela
    a du sens.

    .. [2] https://intra-bocal.epitech.eu/

... accèder aux newsgroups ?
    Les newsgroups ne sont rien de plus que des forums. Il est possible
    d’accéder aux groupes du PIE sur le serveur ``news.epita.fr`` avec un
    client NNTP tel que slrn, rtin, Gnus ou encore Thunderbird, Pan et
    Sylpheed.

    Un tutoriel pas-à-pas sur l’utilisation d’slrn est disponible ici :
    http://canartichaut.kawie.fr/essentiel-configuration-slrn/

... monter une clef USB sans rooter son rack sous Unix ?
    Monter une clef USB avec ``mount(1)`` demande les permissions du
    superutilisateur (root). Le programme ``pmount(1)`` permet heureusement de
    s’en sortir avec un utilisateur normal.::

        # Monte la partition /dev/sdb1
        pmount sdb1

        # Monte la partition s’appelant MyUSB
        pmount LABEL=MyUSB
