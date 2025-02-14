
<html>
    <!-- LOGIN -->
	
	<head>
		<meta http-equiv="X-UA-Compatible" content="IE=Edge" /> <!-- HB-3426 -->
	    <script type="text/javascript" src="js/ophb/main_ophb_0011.js"></script>
	    <script type="text/javascript" src="bibliotecas/jquery/jquery-1.2.6.js"></script>
	    <script type="text/javascript" src="bibliotecas/jqform/jquery.form.js"></script>
	    <script type="text/javascript" src="bibliotecas/validate/jquery.validate.js"></script>
		<script type="text/javascript" src="bibliotecas/jquery/teclado.virtual/jquery.caret.js"></script>
	    <script type="text/javascript" src="bibliotecas/jquery/teclado.virtual/jquery.osk.js"></script>
		<script type="text/javascript" src="bibliotecas/jquery/jquery.event.drag-1.4.min.js"></script>
		<script type="text/javascript" src="js/teclado-virtual-controller.js" charset="utf-8"></script>
		<script type="text/javascript" src="js/transaction-controller.js"></script>
	    <script type="text/javascript" src="js/LinkTransactionController.js"></script>
	    <script type="text/javascript" src="js/link-controller.js"></script>
	    <script type="text/javascript" src="bibliotecas/jquery/jqModal.min.js"></script>
	    <script type="text/javascript" src="js/modal-controller.js"></script>
	    <script type="text/javascript" src="js/JavaScript-Seal-v3.0.js"></script>
        <link rel="stylesheet" href="bibliotecas/css/modal.css" type="text/css" media="all" charset="utf-8"/>
        <link rel="stylesheet" href="bibliotecas/css/link.modal.css" type="text/css" media="all" charset="utf-8"/>
        <link rel="stylesheet" href="componentes/contenidos/estado/estado.css" type="text/css" media="screen" charset="utf-8"/>
        <script type="text/javascript" src="componentes/contenidos/estado/estado.js"></script>
        <script type="text/javascript" src="componentes/contenidos/enlaces.login/enlaces.login.js"></script>
	    <title>Red Link - BANCO DE LA NACION ARGENTINA</title>
		<link rel="stylesheet" type="text/css" href="entidades/banco.nacion.v2/vista/login.css" />
        <link rel="stylesheet" media="print" type="text/css" href="entidades/banco.nacion.v2/vista/toprint.css" />
        <link rel="stylesheet" href="componentes/contenidos/teclado/teclado_full.css" type="text/css" media="screen" charset="utf-8"/>
	
		<!-- tag manager  -->
		
		
		
		
		

		<script type="text/javascript">
            var urlFaqs = 'faqs.htm';
            var urlInformacion = 'informacion.htm';
            var urltyc = 'terminos.htm';
            var urlSeguridad = 'seguridad.htm';
            var usarTecladoVirtual = true;
            var tecladoAlfanum = true;
            var urlLogout = "logouttyc.htm";
            var urlLogin = "login.htm";            
            var urlBrowserError = "browsererror.htm";
            var servicePackBloqueadosIE6 = "";
            var ipSinRestriccionIE6SP1 =  false;
            var pdfFaq = '/bna/faqs/bna.pdf';
            var habilitarRecordarUsuario = false;
            var fiidEntidad = '0011';
            var urlEnrolamientoExterno = '';
            var urlEnrolamiento = 'registrarse.htm';
            var urlRedireccionDesbloqueo = 'desbloqueoSolicitud.htm';
            var urlRedireccionBlanqueo = 'blanqueoSolicitud.htm';
            var isBancoMigrado = 'false';
            var urlBancoMigrado = '';
		</script>
				
	    <script type="text/javascript" src="js/login-utils.js"></script>
	    <script type="text/javascript" src="js/tyc-controller.js"></script>
   		<script type="text/javascript" src="js/sfa-base.js"></script>
   		<script type="text/javascript">
   			validarBancoMigradoController.validarBancoMigrado();
   		</script>
		
			<script async data-insuit-position="right" data-insuit-tab-custom="true" type="text/javascript" src="https://hb.accesible.redlink.com.ar/i4tservice/insuit-app.js"></script> 
		
	</head>
	<body>
		  
		<div id="jqmOverlay"></div>
		<div class="textoClave" id="ayudaUsuario">
			<a href="javascript:;" class="cerrarAyuda" title="Cerrar ayuda">Cerrar</a>
			<br />
			<span>
				<b>&iquest;C&oacute;mo obtengo el usuario y la clave para operar?<br /></b>
				Es muy sencillo, para obtener &quot;Usuario y Clave de HOME BANKING&quot;, debe dirigirse &quot;por &uacute;nica vez&quot; a un Cajero Autom&aacute;tico de la Red Link para obtener su N&uacute;mero de Usuario y elegir su Clave.
				<br /><br />
				<b>&iquest;Qu&eacute; pasos debo seguir para obtener el N&uacute;mero de Usuario y elegir la Clave?</b>
				<br />Los pasos a seguir son los siguientes:
				    <ul>
						<li>Ingresar su Tarjeta y PIN en el Cajero Autom&aacute;tico de la Red Link.</li>
					    <li>Seleccionar la opci&oacute;n &quot;Claves&quot; del men&uacute; principal y en la pr&oacute;xima pantalla elegir &quot;Home Banking-Link Celular&quot;.</li>
					   <li> Ingresar una clave num&eacute;rica de 6 (seis) d&iacute;gitos s&oacute;lo conocida por usted.</li>
					   <li>Reingresar dicha clave.</li>
					   <li> Obtendr&aacute; el ticket de la operaci&oacute;n (el sistema le asignar&aacute; un &quot;N&uacute;mero de Usuario&quot;).</li>
					   <li> Deber&aacute; conservar este ticket ya que los datos que contiene ser&aacute;n necesarios cuando ingrese por primera vez a Home Banking.</li>
					</ul>
			</span>
		</div>
		<div class="textoClave" id="ayudaAvatar">
			<a href="javascript:;" class="cerrarAyudaAvatar" title="Cerrar ayuda">Cerrar</a>
			<br />
			<span>
				La imagen que se visualiza al ingresar el usuario de Home Banking es un nuevo elemento para que Ud. opere m&aacute;s seguro.
				La primera vez que opere en Home Banking debe ingresar y seleccionar una imagen que pueda recordar f&aacute;cilmente. <br />
				IMPORTANTE: si Ud. no visualiza la imagen que configur&oacute; en Home Banking o bien aparece otra imagen, por su seguridad <b>no ingrese la clave. </b>
				Llame inmediatamente al Banco o al Call Center de Red Link al (011) 4319-LINK (5465) &oacute; 0800-888-LINK (5465).
			</span>
		</div>
		<script type="text/javascript">
		//<!--
			$(document).ready(function() {
                var sessionExpired = 'false';                
                if (sessionExpired == 'true') {
                    estado.show('Su sesi&oacute;n ha caducado. Por favor, ingrese nuevamente.', estado.tipo.ERROR);
                }

                var loginTimeout = 'false';
                if (loginTimeout == 'true') {
                    estado.show('No ha sido posible ingresar. Por favor vuelva a intentar en unos minutos.', estado.tipo.ERROR);
                }

                
	            $(document).keydown(function(e) {
	            	if (e.which == 13) {
	            	    ingresar();
		            	return false;
	            	} 
	            });
	        });
	        
            function loginTimeout(data) {
                window.location = 'login.htm?loginTimeout=true';
            }


            if (parent.frames.length) top.location.href= document.location; 
        //-->
		</script>
		<div class="botonera">
            

<!-- CSS -->
<link rel="stylesheet" href="componentes/contenidos/enlaces.login/enlaces.login.css" type="text/css" media="screen" charset="utf-8"/>

<!-- VIEW -->
<div class="enlacesLogin">
	<ul>
        <li>
            <a href="javascript:;" id="faqsLogin" alt='Preguntas Frecuentes' title='Preguntas Frecuentes'>
                Preguntas Frecuentes
            </a>
        </li>
        <li>
            <a href="javascript:;" id="infoLogin" alt='Informaci&oacute;n de Home Banking' title='Informaci&oacute;n de Home Banking'>
                Informaci&oacute;n de Home Banking
            </a>
        </li>
        <li>
            <a href="javascript:;" id="tycLogin" alt='T&eacute;rminos y Condiciones' title='T&eacute;rminos y Condiciones'>
                T&eacute;rminos y Condiciones
            </a>
        </li>        
        <li>
            <a href="javascript:;" id="seguridadLogin" alt='Seguridad del Sistema' title='Seguridad del Sistema'>
                Seguridad del Sistema
            </a>
        </li>

	</ul>	
	<div id="contenedorSeguridad">
		<a href="http://www.bna.com.ar/institucional/consejos_seguridad.asp" id="consejoSeguridad" alt='Consejos de Seguridad' target='_blank' title='Consejos de Seguridad'>
                Consejos de Seguridad
            </a>
	</div>
</div>


<script type="text/javascript" src="componentes/contenidos/enlaces.login/enlaces.login.js"></script>
               
		</div>		
        <form enctype="multipart/form-data" id="UserNameVerificationForm" name="UserNameVerificationForm" method="post" action="doLoginFirstStep.htm">
			<input type="hidden" id="isInclu" name="isInclu" value="false"/>    
			<div style="clear:both;"></div>
			<div id="contenedor" class="contenedor">
		        <div id="recuadroMensaje" class="contEstado ocultar"></div>
		        <!-- fin componente estado -->

				<div class="login" id="loginBox" style="display:none;">
					<div class="bienvenido" id="divLogo"><img src="entidades/banco.nacion.v2/vista/imagenes/login/logo.gif" alt="" /></div>
					<div class="darBienvenida" id="divDarBienvenida" style="display:none;">
							<h2><span id="holaSpan"></span></h2>
							<p class="olvidarUsuario"><a href="javascript:OlvidarUsuLStorage();" ><span id="noSoySpan"></span></a></p>
<!-- 							<input type="checkbox" name="pcCompartida" id="pcCompartida" /> -->
					</div>
					<div class="ingreso" id="divIngreso">
						<div class="siEsPcPublica"  id="divSiEsPcPublica" style="display:none">
							<label for="pcCompartida">Ingrese con Teclado Virtual</label>
							<input type="checkbox" name="pcCompartida" id="pcCompartida" />
						</div>
						<div class="campos" id="divCampos">
                            <div id="campoUsuario">
                                <label for="username">Usuario</label>
							    <div class="campo">
                                    <input type="text" id="usuario" name="username" />    
							    </div>
								<a href="javascript:;" class="preg" id="loginInfoId" title="¿Cómo sacar la clave?">
	                                <img src="entidades/banco.nacion.v2/vista/imagenes/login/preg_circle.gif" alt="?" border="0" />	
	                            </a>
	                            <div class="ctdorCkeckRecordar" style="display:none;"> 
	                            	<input type="checkbox" name="recordarme" id="recordarme"/> 
 									<label id="lblRecordarme" for="recordarme">Quiero recordar mi usuario</label>
 								</div> 
							</div>
							<div id="campoPassword" style="display:none">
		                        <label for="password">Clave</label>
							    <div class="campo">
                                    <input type="password" name="pin" id="clave" />
                                </div>
								<a href="javascript:;" class="preg ayuda2" title="Ayuda para la imagen">
	                                <img src="entidades/banco.nacion.v2/vista/imagenes/login/preg_circle.gif" alt="?" border="0" />
	                            </a>
														
                                <div id="contAvatar" class="avatar" >

                                    <img alt="avatar" />
                                </div>
	                            
							</div>
							<div id="vistaSfa" style="float: none; margin-top:5px">

							</div>
						</div>
					</div>
					<a href="javascript:ingresar();" class="btn_ingresar">Ingresar</a>
					
					
						
							<div id="btnAccesoBloqueado" class="accesoBloqueado">
								<a href="javascript:accesoBloqueadoController.mostrarModal();" class="bloqueado">&iquest;Acceso bloqueado?</a>
							</div>
							
							<div id="accesoBloqueadoModal" class="abModal jqmWindow linkModal" style="display:none">
								<div class="top">
									<h4>&iquest;Acceso bloqueado?</h4>
									<a id="cerrarABModal" href="javascript:;">cerrar</a>
								</div>
								<div class="middle">
									<div class="divAB">
										<label><input id="radioRecordarClave" type="radio" name="seleccion" checked>&iquest;Bloqueaste tu usuario y todav&iacute;a record&aacute;s tu clave de acceso?</label>
									</div>
									<div class="divAB">
										<label><input id="radioNoRecordarClave" type="radio" name="seleccion">&iquest;Bloqueaste tu usuario y no record&aacute;s tu clave de acceso?<br><b>Para usar esta opci&oacute;n, deber&aacute;s tener activo tu Token.</b></label>
									</div>
									<div class="divAB">
										<label><input id="radioNoRecordarUsuario" type="radio" name="seleccion">&iquest;No record&aacute;s tu usuario y necesit&aacute;s uno nuevo?</label>
									</div>
								</div>
								<div class="bottom">
					            	<div class="clave">
					                    <a id="botonCancelar" href="javascript:accesoBloqueadoController.atras();">Atr&aacute;s</a>
					                	<a id="botonAceptar" href="javascript:accesoBloqueadoController.continuar();">Continuar</a>
					                </div>
					            </div>
							</div>
					     	<div id="redireccionATMModal" class="jqmWindow linkModal" style="display:none">
								<div class="top">
									<h4>&iquest;Acceso bloqueado?</h4>
									<a id="cerrarRedireccionATMModal" href="javascript:;">cerrar</a>
								</div>
								<div class="middle">
						            <div id="leyendaTokenActivo" style="text-align: justify">Pod&eacute;s generar tu nuevo usuario en un cajero autom&aacute;tico. Seleccion&aacute; la opci&oacute;n de generaci&oacute;n de clave, e ingres&aacute; una clave num&eacute;rica de 6 d&iacute;gitos. Guard&aacute; el ticket impreso, vas a necesitarlo para crear tu nuevo usuario.</div>
								</div>
								<div class="bottom">
						          	<div class="clave">
						                  <a id="botonAceptar" href="javascript:accesoBloqueadoController.aceptarRedireccionATMModal();">Aceptar</a>
						              </div>
						          </div>
					     	</div>
						    
  						
					
					
					
						
							<div id="btnPrimerVezQueIngresas" class="registrarse">
								<a href="javascript:primerIngresoController.mostrarModal();" class="enrolamiento">&iquest;Primera vez que ingres&aacute;s?</a>
							</div>
							
							<div id="primerIngresoModal" class="abModal jqmWindow linkModal" style="display:none">
								<div class="top">
									<h4>&iquest;Primera vez que ingres&aacute;s?</h4>
									<a id="cerrarPIModal" href="javascript:;">cerrar</a>
								</div>
								<div class="middle">
									<div class="divAB">
										<label><input id="radioNuevoUsuario" type="radio" name="seleccion" checked>&iquest;Ya obtuviste tu nuevo usuario por cajero autom&aacute;tico? Ingres&aacute; con el usuario impreso en el ticket y la clave que elegiste en el cajero.</label>
									</div>
									<div class="divAB">
										<label><input id="radioSinUsuario" type="radio" name="seleccion">Si no has gestionado tu usuario por cajero autom&aacute;tico, gestionalo en este momento por aqu&iacute;. Podr&aacute;s crear tu usuario si nunca antes usaste Home Banking.</label>
									</div>
								</div>
								<div class="bottom">
					            	<div class="clave">
					                    <a id="botonCancelar" href="javascript:primerIngresoController.atras();">Atr&aacute;s</a>
					                	<a id="botonAceptar" href="javascript:primerIngresoController.continuar();">Continuar</a>
					                </div>
					            </div>
							</div>
						    
						
					
					<div class="pie" id="divPie">
							<img src="entidades/banco.nacion.v2/vista/imagenes/login/verisignlogo2.gif" alt="" class="certify right" />
							<img src="entidades/banco.nacion.v2/vista/imagenes/login/csseal_transp_S_v4.gif" alt="" class="certify left" />
					</div>
				</div>
				<div class="cuerpo" id="divCuerpo">
					<p>&quot;ALERTA! Banco Naci&oacute;n, nunca iniciar&aacute; un contacto o conversaci&oacute;n, ni le pedir&aacute; que informe o confirme sus claves, pin, token u otros datos sensibles, a trav&eacute;s de redes sociales, correo electr&oacute;nico, mensaje de WhatsApp, mensaje de texto o llamado telef&oacute;nico&quot;.<br />
<br />
#EVITEMOS LAS ESTAFAS VIRTUALES<br />
<br />
&quot;En caso de haber sufrido una estafa comun&iacute;quese al (011) 4319-5465 (o canal oficial correspondiente)&rdquo;.</p>
					<a href="http://www.redlink.com.ar" target="_blank" class="RedLinkLogoLogin">
						<img src="entidades/banco.nacion.v2/vista/imagenes/login/logo_link.jpg" width="60" height="60" border="0" alt="RED LINK" >
					</a> 
					<div class="chicos" >
						<script src="js/JavaScript-Seal-v3.0.js" type="text/javascript"></script>
						<div align="center" title="Haga Click para Verificar - Este sitio cuenta con un Certificado SSL para asegurar la confidencialidad de sus comunicaciones.">
<!-- 				    <a href="javascript:Seal_Certificado('hb.redlink.com.ar', 'es', 'CURS-3.0', 'imagen');" target="_blank" class="linkCertisur"/> -->
						<a href="https://seal.certisur.com/getseal?host_name=hb.redlink.com.ar&lang=es&version=CURS-3.0&domain=imagen&ca=norton" target="_blank" class="linkCertisur"/>
							<img src="entidades/banco.nacion.v2/vista/imagenes/login/CURS-3.0.png" alt="CertiSur Seal" width="100" height="72" border="0" class="imagenCertisur"/>
						</a>
						</div>
					</div>
					
				</div>
			</div>
		</form>
		
		
        <form enctype="multipart/form-data" id="RestauracionUsuarioForm" name="RestauracionUsuario" method="post" action="">
        </form>
        
        <form enctype="multipart/form-data" id="EnrolamientoForm" name="EnrolamientoForm" method="post" action="">
        </form>
		
		<!-- Modal Ayuda Inclusite -->
		
		<div id="ayudaInclusiteModal" class="jqmWindow linkModal" style="display:none">
			<div id="filtro" class="filtro" style="height: 100%; width: 100%; position: fixed; left: 0px; top: 0px; z-index:1999; opacity: 0.5; filter:alpha(opacity=50); ;"></div>
			<div id="cuerpo" class="divContent" style="z-index:3000; position: absolute;">        		
				<table border="0" style="z-index:5000; border-radius:6px; border:1px solid #999; background-color:#e5e6e6;"  >
				  <tr>
					<td colspan="6" class="tipo2" height="1">&nbsp;</td>
					<td>&nbsp;</td>
				  </tr>
				  <tr>
					<td colspan="7" align="right" valign="top" class="tipo2" ><table width="100%" border="0">
					  <tr>
						<td width="9%">&nbsp;</td>
						<td width="80%"><span class="tipo21">Bienvenido al sitio de Home Banking accesible.<br />
				Los siguientes son los comandos básicos de navegación que usted utilizará en este sitio.<br />
				Ante cualquier duda puede volver a consultarlos presionando F1.</span></td>
						<td width="10%"><a href="javascript:;" id="hideModalAyuda"><span class="tipo2">Cerrar</span></a></td>
						<td width="1%">&nbsp;</td>
					  </tr>
					</table></td>
				  </tr>
				  <tr>
					<td width="14%" height="1" align="right" valign="top" >&nbsp;</td>
					<td height="1" class="tipo1">&nbsp;</td>
					<td width="14%" height="1" align="right" valign="top" >&nbsp;</td>
					<td height="1"  align="left" valign="top" class="tipo1">&nbsp;</td>
					<td width="14%" height="1"  align="right" valign="top" >&nbsp;</td>
					<td height="1" align="left" valign="top" class="tipo1">&nbsp;</td>
					<td height="1">&nbsp;</td>
				  </tr>
				  <tr>
					<td align="right" valign="top" ><img src="images/inclusite/punto.png" width="69" height="66" id="punto"/></td>
					<td width="12%" class="tipo1">Presione la tecla punto para salir del área actual. Pulsa dos veces para volver a la página anterior si estás en 'Áreas'.</td>
					<td width="13%" align="right" valign="top" ><img src="images/inclusite/escape.png" width="69" height="66" id="esc" /></td>
					<td width="13%"  align="left" valign="top" class="tipo1">Presione la tecla Escape para abrir la ventana de configuración de Inclusite.</td>
					<td width="17%"  align="right" valign="top" ><img src="images/inclusite/cero.png" width="69" height="66" id="cero"/></td>
					<td width="16%" align="left" valign="top" class="tipo1">Presione la tecla cero para repetir las opciones.</span></td>
					<td width="5%">&nbsp;</td>
				  </tr>
				  <tr>
					<td height="1" class="margenimagizq">&nbsp;</td>
					<td height="1" align="left" valign="top" class="tipo1">&nbsp;</td>
					<td height="1" style="text-align: right">&nbsp;</td>
					<td height="1">&nbsp;</td>
					<td height="1" class="margenimagizq">&nbsp;</td>
					<td height="1">&nbsp;</td>
					<td height="1">&nbsp;</td>
				  </tr>
				  <tr>
					<td align="right" valign="top" ><img src="images/inclusite/up.png" width="69" height="66" id="up"/></td>
					<td align="left" valign="top" class="tipo1">Presione la tecla de navegación subir para desplazarte hacia arriba dentro de la página web.</td>
					<td  align="right" valign="top" ><img src="images/inclusite/b.png" width="69" height="66" id="b"/></td>
					<td align="left" valign="top" class="tipo1">Presione la tecla B para ir a las áreas de la página web.</td>
					<td align="right" valign="top" ><img src="images/inclusite/1.png" width="69" height="66" id="1"/></td>
					<td width="16%" align="left" valign="top" class="tipo1">Presione el número correspondiente para acceder al área deseada.</span></td>
					<td>&nbsp;</td>
				  </tr>
				  <tr>
					<td height="1" class="margenimagizq">&nbsp;</td>
					<td height="1" align="left" valign="top" class="tipo1">&nbsp;</td>
					<td height="1" style="text-align: right">&nbsp;</td>
					<td height="1">&nbsp;</td>
					<td height="1" class="margenimagizq">&nbsp;</td>
					<td height="1">&nbsp;</td>
					<td height="1">&nbsp;</td>
				  </tr>
				  <tr>
					<td align="right" valign="top" ><img src="images/inclusite/down.png" width="69" height="66" id="down"/></td>
					<td align="left" valign="top" class="tipo1">Presione la tecla de navegación bajar para desplazarte hacia abajo dentro de la página web.</td>
					<td align="right" valign="top" ><img src="images/inclusite/d.png" width="69" height="66" id="d"/></td>
					<td align="left" valign="top" class="tipo1">Presione la tecla D para ir al área principal de la página web.</td>
					<td align="right" valign="top" ><img src="images/inclusite/f1.png" width="69" height="66" id="f1"/></td>
					<td width="16%" align="left" valign="top" class="tipo1">Presione la tecla F1 para abrir o cerrar la ayuda de esta interfaz.</span></td>
					<td>&nbsp;</td>
				  </tr>
				  <tr>
					<td height="1" class="margenimagizq">&nbsp;</td>
					<td height="1" align="left" valign="top" class="tipo1">&nbsp;</td>
					<td height="1" style="text-align: right">&nbsp;</td>
					<td height="1">&nbsp;</td>
					<td height="1" class="margenimagizq">&nbsp;</td>
					<td height="1">&nbsp;</td>
					<td height="1">&nbsp;</td>
				  </tr>
				  <tr>
					<td align="right" valign="top" ><img src="images/inclusite/back.png" width="114" height="66" id="back"/></td>
					<td align="left" valign="top" class="tipo1">Presione la tecla Retroceder para volver a la página anterior.</td>
					<td align="right" valign="top" ><img src="images/inclusite/z.png" width="69" height="66" id="z"/></td>
					<td align="left" valign="top" class="tipo1">Presione la tecla Z para Aumentar o Disminuir.</td>
					<td align="right" valign="top" ><img src="images/inclusite/espaciadora.png" width="114" height="66" id="espaciadora"/></td>
					<td width="16%" align="left" valign="top" class="tipo1">Presione la tecla Barra Espaciadora para pausar o continuar la reproducción del audio del contenido.</td>
					<td>&nbsp;</td>
				  </tr>
				  <tr>
					<td height="1" class="margenimagizq">&nbsp;</td>
					<td height="1" align="left" valign="top" class="tipo1">&nbsp;</td>
					<td height="1" style="text-align: right">&nbsp;</td>
					<td height="1" colspan="2" align="left" valign="top" class="tipo1">&nbsp;</td>
					<td height="1">&nbsp;</td>
					<td height="1">&nbsp;</td>
				  </tr>
				  <tr>
					<td class="margenimagizq">&nbsp;</td>
					<td align="left" valign="top" class="tipo1">&nbsp;</td>
					<td style="text-align: right"><img src="images/inclusite/asterisco.png" width="69" height="66" id="asterisco"/></td>
					<td colspan="2" align="left" valign="top" class="tipo1"><span class="tipo12"><span class="tipo111">Para áreas superiores a 9, presione el asterisco seguido del número identificador del área, y finalice con asterisco. Ejemplo, asterisco 12 asterisco para acceder al área 12.</span></span></span></td>
					<td>&nbsp;</td>
					<td>&nbsp;</td>
				  </tr>
				  <tr>
					<td class="margenimagizq">&nbsp;</td>
					<td align="left" valign="top" class="tipo1">&nbsp;</td>
					<td style="text-align: right">&nbsp;</td>
					<td>&nbsp;</td>
					<td class="margenimagizq">&nbsp;</td>
					<td>&nbsp;</td>
					<td>&nbsp;</td>
				  </tr>
				</table>
			</div>
		</div>
		
		<!-- Fin Modal Ayuda Inclusite -->
		
        <script type="text/javascript">
        addValidators();
        </script>
		
		<!--  modal olvidar usuario -->
		<div id="olvidarUsuario" class="jqmWindow linkModal" style="display:none;">
			<div class="titSeccion">&iquest;Esta seguro que quiere desactivar Recordar Usuario?</div>
													
			<div class="botonesOlvidar">
			 		<a href="javascript:cancelarOlvidar();" class="btn">Cancelar</a>
			 		<a href="javascript:aceptarOlvidar();" class="btn">Si, Desactivar</a>
		 	</div>  
		</div>
		<!--  modal recordar usuario -->
		<div id="aceptarTycOlvidarUsu" class="jqmWindow linkModal" style="display:none">
			<div class="top">
				<h4>T&eacute;rminos y Condiciones</h4>
				<a href="javascript:;" id="cerrarAceptarTycOlvidarUsu"><span>cerrar</span></a>
			</div>
			<div class="middle" id="textoContenidoTycOlvidarUsu">
				La clave personal y todo o cualquier otro mecanismo adicional de autenticaci&oacute;n personal provisto por el Banco tiene el car&aacute;cter de secreto e intransferible y por lo tanto asumo las consecuencias de su divulgaci&oacute;n a terceros. Asimismo, acepto que la aplicaci&oacute;n memorice mi usuario y lo muestre sin ser digitado y brinde parte de informaci&oacute;n sobre mis credenciales de acceso a terceros que utilicen el dispositivo. En ambos casos libero al Banco de toda responsabilidad de que ello se derive.                           
			</div>
			<div class="btnModalTycRecordar">
				<a id="btnCancelar" href="javascript:cancelarRecordarUsu();" class="nomostrar" title="Cancelar">Cancelar</a>
				<a id="btnAceptar" href="javascript:aceptarRecordarUsu();" class="nomostrar" title="Aceptar">Aceptar</a>
			</div>
		</div>
		
		<!-- Enlaces login -->      
        <div id="enlacesModalLogin" class="jqmWindow linkModal" style="display:none">
            <div class="top">
                <h4></h4>
                <a href="javascript:;" id="cerrarEnlacesModalLogin"><span>cerrar</span></a>
            </div>
            <div class="middle" id="textoContenidoEnlaceLogin">                           
            </div>
            <div class="enlacesBottom">
                <a id="print" href="javascript:;" class="nomostrar" title="Imprimir">Imprimir</a>
                <a id="download" href="javascript:;" class="nomostrar" title="Exportar">Descargar</a>
            </div>
        </div>
        <div id="secondstep"></div>
        <form id="exporter" enctype="multipart/form-data" method="POST" action="">
        </form>
    </body>
</html>
