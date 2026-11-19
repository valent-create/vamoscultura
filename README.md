# vamoscultura
nos dedicamos a la organización de eventos y a loa producción audiovisual
{
  "version": 4,
  "proyecto": "Simulador empresarial Vamos Cultura",

  "empresa": {
    "nombre": "Vamos Cultura",
    "eslogan": "La cultura nos une, las ideas nos mueven.",
    "descripcion": "Empresa dedicada a la organización de eventos culturales y a la producción audiovisual para artistas, emprendimientos y comunidades, promoviendo el talento local y la participación cultural.",
    "sector": "Cultural, artístico y audiovisual",
    "ubicacion": {
      "ciudad": "Barrancabermeja",
      "departamento": "Santander",
      "pais": "Colombia"
    },
    "identidadVisual": {
      "emoji": "🪀",
      "colorPrincipal": "#33204F",
      "colorAcento": "#F5C542",
      "tono": [
        "Creativo",
        "Juvenil",
        "Espontáneo",
        "Cercano",
        "Profesional"
      ]
    },
    "publicoObjetivo": [
      "Artistas locales",
      "Emprendedores",
      "Empresas",
      "Comunidades",
      "Organizaciones culturales",
      "Instituciones educativas"
    ]
  },

  "configuracion": {
    "moneda": "COP",
    "periodoFinanciero": "mensual",
    "modeloCalculo": "por_servicio",
    "servicioPrincipal": "produccion_audiovisual",
    "incluirImpuestos": false,
    "incluirFinanciacion": false,
    "permitirEditarDatos": true,
    "actualizarCalculosAutomaticamente": true
  },

  "catalogoClientes": {
    "titulo": "Nuestros servicios",
    "subtitulo": "Creamos experiencias culturales y contenido audiovisual para impulsar el talento local.",
    "mostrarPreciosBase": true,
    "permitirSeleccionMultiple": true,
    "modalidadContratacion": "cotizacion_personalizada",

    "servicios": [
      {
        "id": "eventos_culturales",
        "nombre": "Organización y producción de eventos culturales",
        "precioBase": 900000,
        "unidad": "evento",
        "descripcion": "Planeación, coordinación y producción de festivales, ferias, encuentros artísticos y actividades comunitarias.",
        "incluye": [
          "Planeación del evento",
          "Organización de actividades",
          "Coordinación de la producción",
          "Acompañamiento durante el evento"
        ],
        "complementosDisponibles": [
          "diseno_grafico",
          "fotografia",
          "video_promocional",
          "publicidad",
          "difusion"
        ],
        "precioPersonalizado": true,
        "activo": true
      },
      {
        "id": "produccion_audiovisual",
        "nombre": "Producción audiovisual y cobertura de eventos",
        "precioBase": 3500000,
        "unidad": "proyecto",
        "descripcion": "Fotografía, grabación, edición de videos y creación de contenido audiovisual para eventos.",
        "incluye": [
          "Fotografía",
          "Grabación audiovisual",
          "Edición de videos",
          "Creación de contenido",
          "Cobertura de eventos"
        ],
        "complementosDisponibles": [
          "fotografia_adicional",
          "video_promocional",
          "diseno_grafico",
          "redes_sociales"
        ],
        "precioPersonalizado": true,
        "activo": true
      }
    ],

    "complementos": [
      {
        "id": "diseno_grafico",
        "nombre": "Diseño gráfico",
        "descripcion": "Creación de afiches, invitaciones y piezas visuales.",
        "precio": null,
        "precioTipo": "por_cotizar"
      },
      {
        "id": "fotografia",
        "nombre": "Fotografía adicional",
        "descripcion": "Registro fotográfico complementario para eventos y actividades.",
        "precio": null,
        "precioTipo": "por_cotizar"
      },
      {
        "id": "fotografia_adicional",
        "nombre": "Paquete fotográfico adicional",
        "descripcion": "Mayor cantidad de fotografías editadas.",
        "precio": null,
        "precioTipo": "por_cotizar"
      },
      {
        "id": "video_promocional",
        "nombre": "Video promocional",
        "descripcion": "Producción de videos adicionales para promocionar marcas o eventos.",
        "precio": null,
        "precioTipo": "por_cotizar"
      },
      {
        "id": "publicidad",
        "nombre": "Publicidad y promoción",
        "descripcion": "Apoyo en la promoción de eventos, actividades o proyectos.",
        "precio": null,
        "precioTipo": "por_cotizar"
      },
      {
        "id": "difusion",
        "nombre": "Difusión del evento",
        "descripcion": "Apoyo en la difusión de información y piezas promocionales.",
        "precio": null,
        "precioTipo": "por_cotizar"
      },
      {
        "id": "redes_sociales",
        "nombre": "Manejo de redes sociales",
        "descripcion": "Creación y organización de contenido para redes sociales.",
        "precio": null,
        "precioTipo": "por_cotizar"
      }
    ],

    "reglasPrecio": {
      "formula": "precioBase + complementosCotizados",
      "mostrarPrecioBase": true,
      "mostrarPrecioComplementos": true,
      "mostrarSubtotal": true,
      "mostrarTotal": true,
      "complementosSinPrecio": "requieren_cotizacion",
      "permitirDescuentos": true,
      "requiereAprobacion": true
    }
  },

  "formularioCliente": {
    "titulo": "Cuéntanos qué necesitas",
    "descripcion": "Queremos conocer tu idea para ofrecerte un servicio que se adapte a tus necesidades.",

    "datosPersonales": [
      {
        "id": "nombreCliente",
        "pregunta": "¿Cuál es tu nombre?",
        "tipo": "texto",
        "obligatoria": true
      },
      {
        "id": "contacto",
        "pregunta": "¿Cuál es tu medio de contacto?",
        "tipo": "texto",
        "obligatoria": true
      }
    ],

    "preguntas": [
      {
        "id": "servicio",
        "pregunta": "¿Qué servicio te interesa?",
        "tipo": "seleccion_multiple",
        "opciones": [
          "Organización de eventos culturales",
          "Producción audiovisual",
          "Ambos servicios",
          "Quiero asesoría"
        ],
        "obligatoria": true
      },
      {
        "id": "tipoProyecto",
        "pregunta": "¿Para qué tipo de proyecto necesitas el servicio?",
        "tipo": "seleccion_unica",
        "opciones": [
          "Evento cultural o artístico",
          "Emprendimiento o negocio",
          "Proyecto personal",
          "Actividad comunitaria",
          "Institución educativa",
          "Otro"
        ],
        "obligatoria": true
      },
      {
        "id": "complementos",
        "pregunta": "¿Qué complementos te gustaría incluir?",
        "tipo": "seleccion_multiple",
        "opciones": [
          "Diseño gráfico",
          "Fotografía adicional",
          "Videos promocionales",
          "Manejo de redes sociales",
          "Publicidad y difusión",
          "Ninguno por ahora"
        ],
        "obligatoria": false
      },
      {
        "id": "fecha",
        "pregunta": "¿Cuándo necesitas el servicio?",
        "tipo": "seleccion_unica",
        "opciones": [
          "En los próximos 7 días",
          "En las próximas semanas",
          "En uno o dos meses",
          "Todavía no tengo fecha"
        ],
        "obligatoria": true
      },
      {
        "id": "presupuesto",
        "pregunta": "¿Cuál es tu presupuesto aproximado?",
        "tipo": "seleccion_unica",
        "opciones": [
          "Menos de $500.000",
          "Entre $500.000 y $1.000.000",
          "Entre $1.000.000 y $3.000.000",
          "Más de $3.000.000",
          "Quiero recibir una cotización"
        ],
        "obligatoria": false
      },
      {
        "id": "detalles",
        "pregunta": "Cuéntanos más sobre tu proyecto y lo que esperas recibir.",
        "tipo": "respuesta_abierta",
        "obligatoria": false
      },
      {
        "id": "expectativas",
        "pregunta": "¿Qué resultado esperas obtener con nuestro servicio?",
        "tipo": "respuesta_abierta",
        "obligatoria": false
      }
    ],

    "privacidad": {
      "solicitarConsentimientoTratamientoDatos": true,
      "usoDatos": "Gestionar solicitudes, preparar cotizaciones y contactar al cliente."
    }
  },

  "cotizacion": {
    "modalidad": "personalizada",
    "requiereRevisionHumana": true,
    "permiteContratacionAutomatica": false,

    "pasos": [
      "seleccion_servicios",
      "seleccion_complementos",
      "formulario_cliente",
      "solicitud_recibida",
      "revision_equipo",
      "elaboracion_cotizacion",
      "envio_al_cliente",
      "confirmacion"
    ],

    "resumenPrecios": {
      "mostrarPrecioBase": true,
      "mostrarComplementos": true,
      "mostrarDescuentos": true,
      "mostrarSubtotal": true,
      "mostrarTotal": true,
      "mostrarConceptosPorCotizar": true
    },

    "estados": [
      "borrador",
      "solicitud_recibida",
      "en_revision",
      "cotizacion_enviada",
      "pendiente_de_confirmacion",
      "aceptada",
      "rechazada",
      "finalizada"
    ],

    "datosSolicitud": [
      "nombreCliente",
      "contacto",
      "serviciosSeleccionados",
      "complementosSeleccionados",
      "tipoProyecto",
      "fechaSolicitada",
      "presupuesto",
      "detalles",
      "expectativas"
    ],

    "datosCotizacion": [
      "numeroCotizacion",
      "fechaEmision",
      "fechaVencimiento",
      "servicios",
      "complementos",
      "subtotal",
      "descuentos",
      "total",
      "condiciones",
      "observaciones"
    ],

    "reglas": {
      "noInventarPrecios": true,
      "noCobrarComplementosSinCotizar": true,
      "solicitarAprobacionDelCliente": true,
      "calcularTotalSoloConPreciosConfirmados": true
    }
  },

  "panelAdministrativo": {
    "accesoPrivado": true,
    "funciones": [
      "Consultar solicitudes",
      "Consultar datos de clientes",
      "Revisar servicios seleccionados",
      "Editar precios de complementos",
      "Crear cotizaciones",
      "Aplicar descuentos autorizados",
      "Calcular subtotales y totales",
      "Enviar cotizaciones",
      "Actualizar estados de solicitudes",
      "Consultar historial de cotizaciones"
    ],
    "permisos": {
      "administrador": [
        "ver",
        "crear",
        "editar",
        "cotizar",
        "aprobar",
        "gestionar"
      ]
    }
  },

  "costos": {
    "md": [
      {
        "id": "materiales",
        "nombre": "Materiales y recursos audiovisuales",
        "valor": 900000,
        "frecuencia": "por_unidad",
        "tipo": "variable"
      },
      {
        "id": "transporte",
        "nombre": "Transporte por evento",
        "valor": 50000,
        "frecuencia": "por_unidad",
        "tipo": "variable"
      }
    ],

    "mod": [
      {
        "id": "equipo_produccion",
        "nombre": "Equipo de producción audiovisual",
        "cantidad": 4,
        "valorPorPersona": 400000,
        "frecuencia": "por_unidad",
        "tipo": "variable",
        "incluidoEnCostoPorProyecto": true
      }
    ],

    "cif": [
      {
        "id": "edicion_mantenimiento",
        "nombre": "Editores, mantenimiento y alquiler",
        "valor": 500000,
        "frecuencia": "mensual",
        "tipo": "fijo"
      },
      {
        "id": "almacenamiento",
        "nombre": "Almacenamiento en la nube",
        "valor": 60000,
        "frecuencia": "mensual",
        "tipo": "fijo"
      }
    ],

    "gastos": [
      {
        "id": "publicidad",
        "nombre": "Publicidad y promoción",
        "valor": 600000,
        "frecuencia": "mensual",
        "tipo": "fijo"
      },
      {
        "id": "diversos",
        "nombre": "Gastos diversos",
        "valor": 300000,
        "frecuencia": "mensual",
        "tipo": "fijo"
      }
    ]
  },

  "nomina": {
    "personaJuridica": true,
    "empleados": [
      {
        "id": "administrador",
        "cargo": "Administrador",
        "salarioBaseMensual": 1750905,
        "arl": "II",
        "contratar": true,
        "tipoContrato": "por_definir",
        "costoTotalEmpresaMensual": null,
        "estadoCalculo": "pendiente_de_validar"
      }
    ],
    "observacion": "El costo total del empleador debe incluir los conceptos laborales y aportes aplicables. Se debe validar antes de incorporarlo a los cálculos definitivos."
  },

  "escenarios": {
    "unidad": "proyectos_mensuales",
    "pesimista": 2,
    "base": 3,
    "optimista": 4
  },

  "caja": {
    "capitalInicial": 3000000,
    "moneda": "COP",
    "proyeccionMeses": 6,
    "ventasProyectadas": [4, 4, 6, 6, 6, 7],
    "actualizarSaldoAutomaticamente": true,
    "incluirIngresos": true,
    "incluirCostosVariables": true,
    "incluirCostosFijos": true,
    "alertarSaldoNegativo": true
  },

  "calculos": {
    "estado": "provisional",
    "servicioAnalizado": "produccion_audiovisual",
    "precioVentaPorUnidad": 3500000,
    "costoMaterialesPorUnidad": 950000,
    "costoManoObraPorUnidad": 1600000,
    "costoVariablePorUnidad": 2550000,
    "margenContribucionPorUnidad": 950000,
    "costosFijosMensualesSinNomina": 1460000,
    "salarioBaseAdministrador": 1750905,
    "costosFijosMensualesConSalarioBase": 3210905,
    "puntoEquilibrioUnidades": 4,
    "formulaIngresos": "precioVentaPorUnidad * unidadesVendidas",
    "formulaCostosVariables": "costoVariablePorUnidad * unidadesVendidas",
    "formulaMargen": "precioVentaPorUnidad - costoVariablePorUnidad",
    "formulaUtilidad": "ingresos - costosVariables - costosFijos",
    "formulaPuntoEquilibrio": "redondear_hacia_arriba(costosFijos / margenContribucionPorUnidad)",
    "observacion": "Los cálculos son provisionales. Incluyen el salario base del administrador, pero no las cargas adicionales de nómina, impuestos ni otros conceptos pendientes de validar."
  },

  "simulador": {
    "permitirCambiarPrecios": true,
    "permitirCambiarCostos": true,
    "permitirCambiarVentas": true,
    "recalcularAutomaticamente": true,
    "mostrarIngresos": true,
    "mostrarCostos": true,
    "mostrarUtilidad": true,
    "mostrarPuntoEquilibrio": true,
    "mostrarProyecciones": true,
    "mostrarGraficas": true,
    "mostrarAlertasFinancieras": true,
    "graficas": [
      "Ingresos mensuales",
      "Costos mensuales",
      "Utilidad mensual",
      "Flujo de caja",
      "Comparacion de escenarios"
    ]
  },

  "decision": {
    "numeroClave": "6 eventos mensuales porque permiten generar ganancias.",
    "accion30dias": "Realizar una campaña de promoción digital y presencial mediante Instagram, TikTok, Facebook y visitas a artistas y emprendimientos.",
    "usoCriticoIA": "No se identificaron recomendaciones o cálculos de la IA que se quisieran cambiar durante el ejercicio."
  },

  "reportes": {
    "permitirExportarJSON": true,
    "permitirExportarPDF": true,
    "permitirExportarExcel": true,
    "incluirDatosEmpresa": true,
    "incluirCatalogoServicios": true,
    "incluirCotizaciones": true,
    "incluirResumenFinanciero": true,
    "incluirProyecciones": true
  }
}
