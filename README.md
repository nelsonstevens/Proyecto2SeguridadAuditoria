% Options for packages loaded elsewhere
\PassOptionsToPackage{unicode}{hyperref}
\PassOptionsToPackage{hyphens}{url}
%
\documentclass[
]{article}
\usepackage{lmodern}
\usepackage{amssymb,amsmath}
\usepackage{ifxetex,ifluatex}
\ifnum 0\ifxetex 1\fi\ifluatex 1\fi=0 % if pdftex
  \usepackage[T1]{fontenc}
  \usepackage[utf8]{inputenc}
  \usepackage{textcomp} % provide euro and other symbols
\else % if luatex or xetex
  \usepackage{unicode-math}
  \defaultfontfeatures{Scale=MatchLowercase}
  \defaultfontfeatures[\rmfamily]{Ligatures=TeX,Scale=1}
\fi
% Use upquote if available, for straight quotes in verbatim environments
\IfFileExists{upquote.sty}{\usepackage{upquote}}{}
\IfFileExists{microtype.sty}{% use microtype if available
  \usepackage[]{microtype}
  \UseMicrotypeSet[protrusion]{basicmath} % disable protrusion for tt fonts
}{}
\makeatletter
\@ifundefined{KOMAClassName}{% if non-KOMA class
  \IfFileExists{parskip.sty}{%
    \usepackage{parskip}
  }{% else
    \setlength{\parindent}{0pt}
    \setlength{\parskip}{6pt plus 2pt minus 1pt}}
}{% if KOMA class
  \KOMAoptions{parskip=half}}
\makeatother
\usepackage{xcolor}
\IfFileExists{xurl.sty}{\usepackage{xurl}}{} % add URL line breaks if available
\IfFileExists{bookmark.sty}{\usepackage{bookmark}}{\usepackage{hyperref}}
\hypersetup{
  pdftitle={FIREWALL},
  hidelinks,
  pdfcreator={LaTeX via pandoc}}
\urlstyle{same} % disable monospaced font for URLs
\usepackage{longtable,booktabs}
% Correct order of tables after \paragraph or \subparagraph
\usepackage{etoolbox}
\makeatletter
\patchcmd\longtable{\par}{\if@noskipsec\mbox{}\fi\par}{}{}
\makeatother
% Allow footnotes in longtable head/foot
\IfFileExists{footnotehyper.sty}{\usepackage{footnotehyper}}{\usepackage{footnote}}
\makesavenoteenv{longtable}
\usepackage{graphicx}
\makeatletter
\def\maxwidth{\ifdim\Gin@nat@width>\linewidth\linewidth\else\Gin@nat@width\fi}
\def\maxheight{\ifdim\Gin@nat@height>\textheight\textheight\else\Gin@nat@height\fi}
\makeatother
% Scale images if necessary, so that they will not overflow the page
% margins by default, and it is still possible to overwrite the defaults
% using explicit options in \includegraphics[width, height, ...]{}
\setkeys{Gin}{width=\maxwidth,height=\maxheight,keepaspectratio}
% Set default figure placement to htbp
\makeatletter
\def\fps@figure{htbp}
\makeatother
\setlength{\emergencystretch}{3em} % prevent overfull lines
\providecommand{\tightlist}{%
  \setlength{\itemsep}{0pt}\setlength{\parskip}{0pt}}
\setcounter{secnumdepth}{-\maxdimen} % remove section numbering

\title{\protect\hypertarget{_Toc529637428}{}{}FIREWALL}
\usepackage{etoolbox}
\makeatletter
\providecommand{\subtitle}[1]{% add subtitle to \maketitle
  \apptocmd{\@title}{\par {\large #1 \par}}{}{}
}
\makeatother
\subtitle{(PROYECTO Iii)

\includegraphics[width=5.22014in,height=4.80833in]{media/image1.png}}
\author{}
\date{}

\begin{document}
\maketitle

Sayan Danery Aguirre Guzm??n \textbar{} \textbf{7690-17-7987}

Jitzon Aldahir Mendez Gonzalez \textbar{} \textbf{7690-17-8955}

Nelson Steven Cifuentes Chilin \textbar{} \textbf{7690-17-2711}

SEGURIDAD Y AUDITORIA DE SISTEMAS \textbar{} 05/11/2021

ING. MELVIN CAL??

\hypertarget{documentaciuxf3n-para-administraciuxf3n-de-usuarios-y-las-poluxedticas-implementadas.}{%
\section{\texorpdfstring{Documentaci??n para Administraci??n de usuarios y
las pol??ticas implementadas.
}{Documentaci??n para Administraci??n de usuarios y las pol??ticas implementadas. }}\label{documentaciuxf3n-para-administraciuxf3n-de-usuarios-y-las-poluxedticas-implementadas.}}

\hypertarget{preparando-la-estructura}{%
\subsection{Preparando la estructura}\label{preparando-la-estructura}}

\begin{enumerate}
\def\labelenumi{\arabic{enumi}.}
\item
  Como primer paso se procedi?? a crear el dominio, umg.local
\item
  Se cre?? el bosque.
\item
  Se crearon las estructuras organizativas.
\item
  Dentro de cada estructura se crean los usuarios.
\end{enumerate}

\hypertarget{procedimiento-para-crear-un-usuario}{%
\subsection{Procedimiento para crear un
usuario}\label{procedimiento-para-crear-un-usuario}}

\begin{enumerate}
\def\labelenumi{\arabic{enumi}.}
\item
  Desde la ventana de administrador de servidor podemos tener acceso
  desde la pesta??a ``TOOLS''.
\end{enumerate}

\includegraphics[width=4.03125in,height=2.97935in]{media/image2.png}

\begin{enumerate}
\def\labelenumi{\arabic{enumi}.}
\setcounter{enumi}{1}
\item
  Entramos en la opci??n de ``Active Directory Users and Computers''. En
  dicha ventana podemos crear usuarios y grupos.~
\end{enumerate}

\includegraphics[width=3.83543in,height=2.86458in]{media/image3.png}

\begin{enumerate}
\def\labelenumi{\arabic{enumi}.}
\setcounter{enumi}{2}
\item
  En las opciones del dominio nos dirigimos a la carpeta ``Users'', ah??
  podremos ver los usuarios y grupos. Estos est??n representados por un
  icono de una sola persona y otro icono de varias personas, el icono de
  una sola persona significa ``Usuario'' y el de varias personas
  significa ``Grupos''. Como se muestra en la imagen.
\end{enumerate}

\includegraphics[width=3.89583in,height=2.89753in]{media/image4.png}

\begin{enumerate}
\def\labelenumi{\arabic{enumi}.}
\setcounter{enumi}{3}
\item
  En esta misma secci??n, podemos agregar los usuarios o grupos, le damos
  ``click'' en las opciones que se nos ofrecen en la parte superior de
  la ventana.
\end{enumerate}

\includegraphics[width=3.91667in,height=2.9375in]{media/image5.png}

\begin{enumerate}
\def\labelenumi{\arabic{enumi}.}
\setcounter{enumi}{4}
\item
  Al dar click en a??adir un usuario se nos muestra una ventana en donde
  a??adimos la informaci??n del usuario que deseamos agregar.~ Despu??s de
  llenar los campos, elegimos ``siguiente'' y procedemos a crear la
  contrase??a.~
\end{enumerate}

\includegraphics[width=3.9749in,height=2.96875in]{media/image6.png}

\begin{enumerate}
\def\labelenumi{\arabic{enumi}.}
\setcounter{enumi}{5}
\item
  Esta contrase??a puede ser creada para darle al usuario un primer
  ingreso luego podemos pedir que la contrase??a sea re-establecida en el
  primer ingreso. Luego finalizamos dando click en ``finalizar'' y ya
  con esto hemos creado el usuario.
\end{enumerate}

\includegraphics[width=3.8125in,height=2.83555in]{media/image7.png}

\begin{enumerate}
\def\labelenumi{\arabic{enumi}.}
\setcounter{enumi}{6}
\item
  Luego introducimos la informaci??n del grupo ``nombre'' por ejemplo,
  tambi??n podemos elegir las configuraciones del grupo que estamos
  creando. Si deseamos a??adir usuarios al grupo que creamos, damos
  ``click derecho'' sobre el usuario (en este caso el usuario que
  creamos anteriormente).
\end{enumerate}

\includegraphics[width=4.05208in,height=3.03906in]{media/image8.png}

x

\begin{enumerate}
\def\labelenumi{\arabic{enumi}.}
\setcounter{enumi}{7}
\item
  Buscamos la pesta??a de propiedades, y accedemos, una vez dentro,
  buscamos la opci??n de ``miembro de''.~
\end{enumerate}

\includegraphics[width=3.97917in,height=2.97194in]{media/image9.png}

\begin{enumerate}
\def\labelenumi{\arabic{enumi}.}
\setcounter{enumi}{8}
\item
  ~Es aqu?? donde podemos a??adir el usuario al grupo de creamos
  previamente. Damos clic en ``a??adir'' y buscamos el grupo (tambi??n
  podemos escribir el nombre del grupo que creamos) y damos click en
  aceptar (para a??adir el usuario al grupo). Ya el usuario pasa a ser
  miembro del grupo.
\end{enumerate}

\includegraphics[width=3.95833in,height=2.98112in]{media/image10.png}

\hypertarget{lista-de-roles}{%
\subsection{Lista de Roles}\label{lista-de-roles}}

Se crearon unidades organizacionales, siendo las siguientes:

\begin{itemize}
\item
  Contabilidad
\item
  T??cnicos
\item
  Administraci??n
\end{itemize}

\hypertarget{diagrama-del-negocio}{%
\subsection{\texorpdfstring{Diagrama del Negocio
}{Diagrama del Negocio }}\label{diagrama-del-negocio}}

\hypertarget{section}{%
\subsection{}\label{section}}

\hypertarget{poluxedticas-de-los-roles}{%
\subsection{Pol??ticas de los Roles}\label{poluxedticas-de-los-roles}}

\hypertarget{restricciones-estuxe1ndar}{%
\subsubsection{Restricciones Est??ndar}\label{restricciones-estuxe1ndar}}

\textbf{General}

\hypertarget{detalles}{%
\paragraph{Detalles}\label{detalles}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\begin{minipage}[b]{0.47\columnwidth}\raggedright
\hypertarget{dominio}{%
\paragraph{Dominio}\label{dominio}}\strut
\end{minipage} & \begin{minipage}[b]{0.47\columnwidth}\raggedright
\hypertarget{umg.local}{%
\paragraph{umg.local}\label{umg.local}}\strut
\end{minipage}\tabularnewline
\midrule
\endhead
\begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{propietario}{%
\paragraph{Propietario}\label{propietario}}\strut
\end{minipage} & \begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{umgadmin.-del-domino}{%
\paragraph{UMG\textbackslash Admin. del
domino}\label{umgadmin.-del-domino}}\strut
\end{minipage}\tabularnewline
\begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{estado-de-gpo}{%
\paragraph{Estado de GPO}\label{estado-de-gpo}}\strut
\end{minipage} & \begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{habilitado}{%
\paragraph{Habilitado}\label{habilitado}}\strut
\end{minipage}\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{esta-lista-solo-incluye-vuxednculos-en-el-dominio-del-gpo.}{%
\paragraph{Esta lista solo incluye v??nculos en el dominio del
GPO.}\label{esta-lista-solo-incluye-vuxednculos-en-el-dominio-del-gpo.}}

\hypertarget{section-1}{%
\paragraph{}\label{section-1}}

\hypertarget{vuxednculos}{%
\paragraph{V??nculos}\label{vuxednculos}}

\begin{longtable}[]{@{}llll@{}}
\toprule
\textbf{Ubicaci??n} & \textbf{Aplicado} & \textbf{Estado de vinculo} &
\textbf{Ruta}\tabularnewline
\midrule
\endhead
TECNICOS & Si & Habilitado & umg.local/TECNICOS\tabularnewline
ADMINISTRACION & Si & Habilitado &
umg.local/ADMINISTRACION\tabularnewline
VENTAS & Si & Habilitado & umg.local/VENTAS\tabularnewline
& & &\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{section-2}{%
\paragraph{}\label{section-2}}

\hypertarget{section-3}{%
\paragraph{}\label{section-3}}

\hypertarget{section-4}{%
\paragraph{}\label{section-4}}

\hypertarget{section-5}{%
\paragraph{}\label{section-5}}

\textbf{Configuraci??n del equipo}

\hypertarget{directivas-de-cuenta-directiva-de-contraseuxf1as}{%
\paragraph{Directivas de cuenta / Directiva de
Contrase??as}\label{directivas-de-cuenta-directiva-de-contraseuxf1as}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Las contrase??as deben cumplir los requisitos de complejidad &
Habilitado\tabularnewline
Longitud m??nima de la contrase??a & 7 Caracteres\tabularnewline
Vigencia m??xima de la contrase??a & 45 d??as\tabularnewline
Vigencia m??nima de la contrase??a & 30 d??as\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{section-6}{%
\paragraph{}\label{section-6}}

\hypertarget{section-7}{%
\paragraph{}\label{section-7}}

\textbf{Configuraci??n del usuario}

\hypertarget{section-8}{%
\paragraph{}\label{section-8}}

\hypertarget{componentes-de-windows-internet-explorer}{%
\paragraph{Componentes de Windows / Internet
Explorer}\label{componentes-de-windows-internet-explorer}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Impedir el cambio de configuraci??n de proxy & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{section-9}{%
\paragraph{}\label{section-9}}

\hypertarget{componentes-de-windowswindows-update}{%
\paragraph{Componentes de Windows/Windows
Update}\label{componentes-de-windowswindows-update}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Quitar el acceso a todas las caracter??sticas de Windows Update &
Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{menuxfa-inicio-y-barra-de-tareas}{%
\paragraph{Men?? Inicio y barra de
tareas}\label{menuxfa-inicio-y-barra-de-tareas}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Quitar v??nculos y accesos a Windows Update & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{panel-de-controlagregar-o-quitar-programas}{%
\paragraph{Panel de control/Agregar o quitar
programas}\label{panel-de-controlagregar-o-quitar-programas}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Ocultar la opci??n "Agregar programas desde la red" &
Habilitado\tabularnewline
Ocultar la opci??n "Agregar programas desde Microsoft" &
Habilitado\tabularnewline
Ocultar la opci??n "Agregar un programa desde un CD-ROM o disquete &
Habilitado\tabularnewline
Ocultar la p??gina Agregar nuevos programas & Habilitado\tabularnewline
Ocultar la p??gina Agregar o quitar componentes de Windows &
Habilitado\tabularnewline
Ocultar la p??gina Cambiar o quitar programas & Habilitado\tabularnewline
Ocultar la p??gina Configurar acceso y programas predeterminados &
Habilitado\tabularnewline
Quitar Agregar o quitar programas & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{panel-de-controlpersonalizaciuxf3n}{%
\paragraph{Panel de
control/Personalizaci??n}\label{panel-de-controlpersonalizaciuxf3n}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Habilitar protector de pantalla & Habilitado\tabularnewline
Impedir cambiar el color y la apariencia & Habilitado\tabularnewline
Impedir cambiar el fondo de pantalla & Habilitado\tabularnewline
Impedir cambiar el protector de pantalla & Habilitado\tabularnewline
Impedir cambiar iconos del escritorio & Habilitado\tabularnewline
Impedir cambiar punteros del mouse & Habilitado\tabularnewline
Impedir cambiar sonidos & Habilitado\tabularnewline
Proteger el protector de pantalla mediante contrase??a &
Habilitado\tabularnewline
Tiempo de espera del protector de pantalla & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{redconexiones-de-red}{%
\paragraph{Red/Conexiones de red}\label{redconexiones-de-red}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Capacidad para habilitar o deshabilitar una conexi??n LAN &
Deshabilitado\tabularnewline
Prohibir el acceso a las propiedades de componentes de una conexi??n LAN
& Habilitado\tabularnewline
Prohibir el acceso a las propiedades de una conexi??n LAN &
Habilitado\tabularnewline
Prohibir la configuraci??n TCP/IP avanzada & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{sistema}{%
\paragraph{Sistema}\label{sistema}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Actualizaciones autom??ticas de Windows & Deshabilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{sistemaacceso-de-almacenamiento-extrauxedble}{%
\paragraph{Sistema/Acceso de almacenamiento
extra??ble}\label{sistemaacceso-de-almacenamiento-extrauxedble}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Todas las clases de almacenamiento extra??ble: denegar acceso a todo &
Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{sistemaadministraciuxf3n-de-energuxeda}{%
\paragraph{Sistema/Administraci??n de
energ??a}\label{sistemaadministraciuxf3n-de-energuxeda}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Solicitar contrase??a al reanudar tras hibernaci??n o suspensi??n &
Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{sistemadirectiva-de-grupo}{%
\paragraph{Sistema/Directiva de grupo}\label{sistemadirectiva-de-grupo}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\begin{minipage}[b]{0.47\columnwidth}\raggedright
\hypertarget{directiva}{%
\subsection{Directiva}\label{directiva}}\strut
\end{minipage} & \begin{minipage}[b]{0.47\columnwidth}\raggedright
\hypertarget{configuraciuxf3n}{%
\subsection{\texorpdfstring{Configuraci??n
}{Configuraci??n }}\label{configuraciuxf3n}}\strut
\end{minipage}\tabularnewline
\midrule
\endhead
\begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{desactivar-la-actualizaciuxf3n-automuxe1tica-de-los-archivos-adm}{%
\subsection{Desactivar la actualizaci??n autom??tica de los archivos
ADM}\label{desactivar-la-actualizaciuxf3n-automuxe1tica-de-los-archivos-adm}}\strut
\end{minipage} & \begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{habilitado-1}{%
\subsection{Habilitado}\label{habilitado-1}}\strut
\end{minipage}\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{sistemaservicios-de-configuraciuxf3n-regional}{%
\paragraph{Sistema/Servicios de configuraci??n
regional}\label{sistemaservicios-de-configuraciuxf3n-regional}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Denegar el cambio de ubicaci??n geogr??fica & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{restricciones-gerencia}{%
\subsubsection{Restricciones Gerencia}\label{restricciones-gerencia}}

\hypertarget{section-10}{%
\subsection{}\label{section-10}}

\textbf{General}

\hypertarget{detalles-1}{%
\paragraph{Detalles}\label{detalles-1}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\begin{minipage}[b]{0.47\columnwidth}\raggedright
\hypertarget{dominio-1}{%
\paragraph{Dominio}\label{dominio-1}}\strut
\end{minipage} & \begin{minipage}[b]{0.47\columnwidth}\raggedright
\hypertarget{umg.local-1}{%
\paragraph{umg.local}\label{umg.local-1}}\strut
\end{minipage}\tabularnewline
\midrule
\endhead
\begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{propietario-1}{%
\paragraph{Propietario}\label{propietario-1}}\strut
\end{minipage} & \begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{umgadmins.-del-domino}{%
\paragraph{UMG\textbackslash Admins. del
domino}\label{umgadmins.-del-domino}}\strut
\end{minipage}\tabularnewline
\begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{estado-de-gpo-1}{%
\paragraph{Estado de GPO}\label{estado-de-gpo-1}}\strut
\end{minipage} & \begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{habilitado-2}{%
\paragraph{Habilitado}\label{habilitado-2}}\strut
\end{minipage}\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{vuxednculos-1}{%
\paragraph{\texorpdfstring{V??nculos }{V??nculos }}\label{vuxednculos-1}}

\begin{longtable}[]{@{}llll@{}}
\toprule
\textbf{Ubicaci??n} & \textbf{Aplicado} & \textbf{Estado de v??nculo} &
\textbf{Ruta}\tabularnewline
\midrule
\endhead
GERENCIA & Si & Habilitado & umg.local/GERENCIA\tabularnewline
\bottomrule
\end{longtable}

Esta lista solo incluye v??nculos en el dominio del GPO.

\textbf{Configuraci??n del equipo}

\hypertarget{directivas-de-cuenta-directiva-de-contraseuxf1as-1}{%
\paragraph{Directivas de cuenta / Directiva de
Contrase??as}\label{directivas-de-cuenta-directiva-de-contraseuxf1as-1}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Las contrase??as deben cumplir los requisitos de complejidad &
Habilitado\tabularnewline
Longitud m??nima de la contrase??a & 7 caracteres\tabularnewline
Vigencia m??xima de la contrase??a & 45 d??as\tabularnewline
Vigencia m??nima de la contrase??a & 30 d??as\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{componentes-de-windows-internet-explorer-1}{%
\paragraph{Componentes de Windows / Internet
Explorer}\label{componentes-de-windows-internet-explorer-1}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Impedir el cambio de configuraci??n de proxy & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{section-11}{%
\subsection{}\label{section-11}}

\hypertarget{section-12}{%
\subsubsection{}\label{section-12}}

\hypertarget{restricciones-muxe1ximas}{%
\subsubsection{Restricciones M??ximas}\label{restricciones-muxe1ximas}}

\textbf{Visitas}

Se cre?? el perfil de visitas el cual solo permitir?? conectarse seg??n los
siguientes par??metros establecidos:

\begin{itemize}
\item
  Horario - Lunes a S??bado de 8:00 horas a 18:00 horas.
\item
  No se permitir??n conexiones remotas dentro de la red.
\item
  El l??mite para sesiones inactivas ser?? de 5 minutos.
\item
  Para sesiones activas ser?? de 1 hora.
\item
  Para finalizar sesi??n desconectada ser?? de 10 minutos.
\item
  No tendr?? acceso a dispositivos de almacenamiento.
\end{itemize}

\hypertarget{section-13}{%
\subsection{}\label{section-13}}

\textbf{General}

\hypertarget{detalles-2}{%
\paragraph{Detalles}\label{detalles-2}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\begin{minipage}[b]{0.47\columnwidth}\raggedright
\hypertarget{dominio-2}{%
\paragraph{Dominio}\label{dominio-2}}\strut
\end{minipage} & \begin{minipage}[b]{0.47\columnwidth}\raggedright
\hypertarget{umg.local-2}{%
\paragraph{umg.local}\label{umg.local-2}}\strut
\end{minipage}\tabularnewline
\midrule
\endhead
\begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{propietario-2}{%
\paragraph{Propietario}\label{propietario-2}}\strut
\end{minipage} & \begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{umgadmins.-del-domino-1}{%
\paragraph{UMG\textbackslash Admins. del
domino}\label{umgadmins.-del-domino-1}}\strut
\end{minipage}\tabularnewline
\begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{estado-de-gpo-2}{%
\paragraph{Estado de GPO}\label{estado-de-gpo-2}}\strut
\end{minipage} & \begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{habilitado-3}{%
\paragraph{Habilitado}\label{habilitado-3}}\strut
\end{minipage}\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{vuxednculos-2}{%
\paragraph{V??nculos}\label{vuxednculos-2}}

\begin{longtable}[]{@{}llll@{}}
\toprule
\textbf{Ubicaci??n} & \textbf{Aplicado} & \textbf{Estado de v??nculo} &
\textbf{Ruta}\tabularnewline
\midrule
\endhead
VISITAS & Si & Habilitado & umg.local/VISITAS\tabularnewline
\bottomrule
\end{longtable}

Esta lista solo incluye v??nculos en el dominio del GPO.

\hypertarget{section-14}{%
\subsection{}\label{section-14}}

\textbf{Configuraci??n del usuario}

\hypertarget{active-desktopactive-desktop}{%
\paragraph{Active Desktop/Active
Desktop}\label{active-desktopactive-desktop}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\begin{minipage}[b]{0.47\columnwidth}\raggedright
\hypertarget{directiva-1}{%
\subsection{Directiva}\label{directiva-1}}\strut
\end{minipage} & \begin{minipage}[b]{0.47\columnwidth}\raggedright
\hypertarget{configuraciuxf3n-1}{%
\subsection{Configuraci??n}\label{configuraciuxf3n-1}}\strut
\end{minipage}\tabularnewline
\midrule
\endhead
Deshabilitar todos los elementos & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{section-15}{%
\subsection{}\label{section-15}}

\hypertarget{carpetas-compartidas}{%
\paragraph{Carpetas Compartidas}\label{carpetas-compartidas}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Permitir publicaci??n de carpetas compartidas &
Deshabilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{section-16}{%
\subsection{}\label{section-16}}

\hypertarget{componentes-de-windowsinternet-explorer}{%
\paragraph{Componentes de Windows/Internet
Explorer}\label{componentes-de-windowsinternet-explorer}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Impedir el cambio de configuraci??n de proxy & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{componentes-de-windowswindows-update-1}{%
\paragraph{Componentes de Windows/Windows
Update}\label{componentes-de-windowswindows-update-1}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Quitar el acceso a todas las caracter??sticas de Windows Update &
Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{section-17}{%
\paragraph{}\label{section-17}}

\hypertarget{panel-de-control}{%
\paragraph{Panel de Control}\label{panel-de-control}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Ocultar los elementos especificados del Panel de control &
Habilitado\tabularnewline
Prohibir el acceso a Configuraci??n de PC y a Panel de control &
Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{panel-de-controlpersonalizaciuxf3n-1}{%
\paragraph{Panel de
control/Personalizaci??n}\label{panel-de-controlpersonalizaciuxf3n-1}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Habilitar protector de pantalla & Habilitado\tabularnewline
Impedir cambiar el color y la apariencia & Habilitado\tabularnewline
Impedir cambiar el estilo visual de ventanas y botones &
Habilitado\tabularnewline
Impedir cambiar el fondo de pantalla & Habilitado\tabularnewline
Impedir cambiar el protector de pantalla & Habilitado\tabularnewline
Impedir cambiar el tema & Habilitado\tabularnewline
Proteger el protector de pantalla mediante contrase??a &
Habilitado\tabularnewline
Tiempo de espera del protector de pantalla & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{redconexiones-de-red-1}{%
\paragraph{Red/Conexiones de red}\label{redconexiones-de-red-1}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Prohibir el acceso a las propiedades de componentes de una conexi??n LAN
& Habilitado\tabularnewline
Prohibir el acceso a las propiedades de una conexi??n LAN &
Habilitado\tabularnewline
Prohibir el acceso a propiedades de componentes de una conexi??n de
acceso remoto & Habilitado\tabularnewline
Prohibir el acceso al Asistente para nueva conexi??n &
Habilitado\tabularnewline
Prohibir el acceso al elemento Configuraci??n avanzada en el men??
Opciones avanzadas & Habilitado\tabularnewline
Prohibir el acceso al elemento Preferencias de acceso remoto en el men??
Opciones avanzadas & Habilitado\tabularnewline
Prohibir el cambio de nombre de conexiones de acceso remoto privadas &
Habilitado\tabularnewline
Prohibir el cambio de propiedades de una conexi??n de acceso remoto
privada & Habilitado\tabularnewline
Prohibir la adici??n y eliminaci??n de componentes de una LAN o una
conexi??n de acceso remoto & Habilitado\tabularnewline
Prohibir la conexi??n y desconexi??n de una conexi??n de acceso remoto &
Habilitado\tabularnewline
Prohibir la configuraci??n TCP/IP avanzada & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{sistema-1}{%
\paragraph{Sistema}\label{sistema-1}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Impedir el acceso a herramientas de edici??n del Registro &
Habilitado\tabularnewline
Impedir el acceso al s??mbolo del sistema & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{sistemaacceso-de-almacenamiento-extrauxedble-1}{%
\paragraph{Sistema/Acceso de almacenamiento
extra??ble}\label{sistemaacceso-de-almacenamiento-extrauxedble-1}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
CD y DVD: denegar acceso de escritura & Habilitado\tabularnewline
CD y DVD: denegar acceso de lectura & Habilitado\tabularnewline
Discos extra??bles: denegar acceso de escritura &
Habilitado\tabularnewline
Discos extra??bles: denegar acceso de lectura & Habilitado\tabularnewline
Todas las clases de almacenamiento extra??ble: denegar acceso a todo &
Habilitado\tabularnewline
Unidades de disquete: denegar acceso de escritura &
Habilitado\tabularnewline
Unidades de disquete: denegar acceso de lectura &
Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{sistemaadministraciuxf3n-de-comunicaciones-de-internetconfiguraciuxf3n-de-comunicaciones-de-internet}{%
\paragraph{Sistema/Administraci??n de comunicaciones de
Internet/Configuraci??n de comunicaciones de
Internet}\label{sistemaadministraciuxf3n-de-comunicaciones-de-internetconfiguraciuxf3n-de-comunicaciones-de-internet}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Desactivar el acceso a la Tienda & Habilitado\tabularnewline
Desactivar el servicio de asociaciones de archivo de Internet &
Habilitado\tabularnewline
Desactivar Windows Online & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{sistemainstalaciuxf3n-de-controladores}{%
\paragraph{Sistema/Instalaci??n de
controladores}\label{sistemainstalaciuxf3n-de-controladores}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Desactivar la intervenci??n del usuario en b??squedas de controladores de
dispositivo en Windows Update & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{sistemaopciones-de-ctrlaltsupr}{%
\paragraph{Sistema/Opciones de
Ctrl+Alt+Supr}\label{sistemaopciones-de-ctrlaltsupr}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Quitar Administrador de tareas & Habilitado\tabularnewline
Quitar Cerrar sesi??n & Habilitado\tabularnewline
Quitar el bloqueo de equipos & Habilitado\tabularnewline
Quitar la opci??n Cambiar contrase??a & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{sistemaservicios-de-configuraciuxf3n-regional-1}{%
\paragraph{Sistema/Servicios de configuraci??n
regional}\label{sistemaservicios-de-configuraciuxf3n-regional-1}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Denegar el cambio de ubicaci??n geogr??fica & Habilitado\tabularnewline
Denegar la invalidaci??n de configuraciones regionales por parte del
usuario & Habilitado\tabularnewline
Limitar configuraciones regionales del usuario &
Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{section-18}{%
\subsubsection{}\label{section-18}}

\hypertarget{restricciones-sistemas}{%
\subsubsection{Restricciones Sistemas}\label{restricciones-sistemas}}

\textbf{General}

\hypertarget{detalles-3}{%
\paragraph{Detalles}\label{detalles-3}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\begin{minipage}[b]{0.47\columnwidth}\raggedright
\hypertarget{dominio-3}{%
\paragraph{Dominio}\label{dominio-3}}\strut
\end{minipage} & \begin{minipage}[b]{0.47\columnwidth}\raggedright
\hypertarget{umg.local-3}{%
\paragraph{umg.local}\label{umg.local-3}}\strut
\end{minipage}\tabularnewline
\midrule
\endhead
\begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{propietario-3}{%
\paragraph{Propietario}\label{propietario-3}}\strut
\end{minipage} & \begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{umgadmins.-del-domino-2}{%
\paragraph{UMG\textbackslash Admins. del
domino}\label{umgadmins.-del-domino-2}}\strut
\end{minipage}\tabularnewline
\begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{estado-de-gpo-3}{%
\paragraph{Estado de GPO}\label{estado-de-gpo-3}}\strut
\end{minipage} & \begin{minipage}[t]{0.47\columnwidth}\raggedright
\hypertarget{habilitado-4}{%
\paragraph{Habilitado}\label{habilitado-4}}\strut
\end{minipage}\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{vuxednculos-3}{%
\paragraph{V??nculos}\label{vuxednculos-3}}

\begin{longtable}[]{@{}llll@{}}
\toprule
\textbf{Ubicaci??n} & \textbf{Aplicado} & \textbf{Estado de v??nculo} &
\textbf{Ruta}\tabularnewline
\midrule
\endhead
SISTEMAS & Si & Habilitado & umg.local/SISTEMAS\tabularnewline
\bottomrule
\end{longtable}

Esta lista solo incluye v??nculos en el dominio del GPO.

\textbf{Configuraci??n del equipo}

\hypertarget{directivas-de-cuenta-directiva-de-contraseuxf1as-2}{%
\paragraph{Directivas de cuenta / Directiva de
Contrase??as}\label{directivas-de-cuenta-directiva-de-contraseuxf1as-2}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Las contrase??as deben cumplir los requisitos de complejidad &
Habilitado\tabularnewline
Longitud m??nima de la contrase??a & 7 Caracteres\tabularnewline
Vigencia m??xima de la contrase??a & 45 d??as\tabularnewline
Vigencia m??nima de la contrase??a & 30 d??as\tabularnewline
\bottomrule
\end{longtable}

\textbf{Configuraci??n del usuario}

\hypertarget{componentes-de-windowsinternet-explorer-1}{%
\paragraph{Componentes de Windows/Internet
Explorer}\label{componentes-de-windowsinternet-explorer-1}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Impedir el cambio de configuraci??n de proxy & Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{componentes-de-windowswindows-update-2}{%
\paragraph{Componentes de Windows/Windows
Update}\label{componentes-de-windowswindows-update-2}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Quitar el acceso a todas las caracter??sticas de Windows Update &
Habilitado\tabularnewline
\bottomrule
\end{longtable}

\hypertarget{panel-de-controlpersonalizaciuxf3n-2}{%
\paragraph{Panel de
control/Personalizaci??n}\label{panel-de-controlpersonalizaciuxf3n-2}}

\begin{longtable}[]{@{}ll@{}}
\toprule
\textbf{Directiva} & \textbf{Configuraci??n}\tabularnewline
\midrule
\endhead
Habilitar protector de pantalla & Habilitado\tabularnewline
Impedir cambiar el color y la apariencia & Habilitado\tabularnewline
Impedir cambiar el estilo visual de ventanas y botones &
Habilitado\tabularnewline
Impedir cambiar el fondo de pantalla & Habilitado\tabularnewline
Impedir cambiar el protector de pantalla & Habilitado\tabularnewline
Impedir cambiar el tema & Habilitado\tabularnewline
Impedir cambiar iconos del escritorio & Habilitado\tabularnewline
Impedir cambiar la combinaci??n de colores & Habilitado\tabularnewline
Impedir cambiar punteros del mouse & Habilitado\tabularnewline
Impedir cambiar sonidos & Habilitado\tabularnewline
Prohibir seleccionar el tama??o de fuente del estilo visual &
Habilitado\tabularnewline
Proteger el protector de pantalla mediante contrase??a &
Habilitado\tabularnewline
Tiempo de espera del protector de pantalla & Habilitado\tabularnewline
\bottomrule
\end{longtable}

N??mero de segundos de espera hasta que se active el protector de
pantalla -- 300 Segundos.

\end{document}
