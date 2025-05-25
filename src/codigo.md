import '/flutter_flow/flutter_flow_animations.dart';
import '/flutter_flow/flutter_flow_icon_button.dart';
import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import '/flutter_flow/flutter_flow_widgets.dart';
import 'dart:math';
import 'dart:ui';
import '/index.dart';
import 'package:flutter/material.dart';
import 'package:flutter/scheduler.dart';
import 'package:flutter_animate/flutter_animate.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:provider/provider.dart';

import 'pagina_confirmacao_model.dart';
export 'pagina_confirmacao_model.dart';

class PaginaConfirmacaoWidget extends StatefulWidget {
  const PaginaConfirmacaoWidget({super.key});

  static String routeName = 'PaginaConfirmacao';
  static String routePath = '/paginaConfirmacao';

  @override
  State<PaginaConfirmacaoWidget> createState() =>
      _PaginaConfirmacaoWidgetState();
}

class _PaginaConfirmacaoWidgetState extends State<PaginaConfirmacaoWidget>
    with TickerProviderStateMixin {
  late PaginaConfirmacaoModel _model;

  final scaffoldKey = GlobalKey<ScaffoldState>();

  final animationsMap = <String, AnimationInfo>{};

  @override
  void initState() {
    super.initState();
    _model = createModel(context, () => PaginaConfirmacaoModel());

    animationsMap.addAll({
      'containerOnPageLoadAnimation': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 1.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.8, 0.8),
            end: Offset(1.0, 1.0),
          ),
          RotateEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: 1.25,
            end: 1.0,
          ),
        ],
      ),
      'iconOnPageLoadAnimation': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 200.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 300.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.8, 0.8),
            end: Offset(1.0, 1.0),
          ),
          RotateEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 300.0.ms,
            begin: 0.75,
            end: 1.0,
          ),
        ],
      ),
      'textOnPageLoadAnimation1': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 100.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 100.0.ms,
            duration: 300.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 100.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.8, 0.8),
            end: Offset(1.0, 1.0),
          ),
          MoveEffect(
            curve: Curves.easeInOut,
            delay: 100.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.0, 40.0),
            end: Offset(0.0, 0.0),
          ),
        ],
      ),
      'textOnPageLoadAnimation2': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 150.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 150.0.ms,
            duration: 300.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 150.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.8, 0.8),
            end: Offset(1.0, 1.0),
          ),
          MoveEffect(
            curve: Curves.easeInOut,
            delay: 150.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.0, 40.0),
            end: Offset(0.0, 0.0),
          ),
        ],
      ),
      'textOnPageLoadAnimation3': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 200.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 300.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.8, 0.8),
            end: Offset(1.0, 1.0),
          ),
          MoveEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.0, 40.0),
            end: Offset(0.0, 0.0),
          ),
        ],
      ),
      'buttonOnPageLoadAnimation': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 250.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 250.0.ms,
            duration: 300.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 250.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.8, 0.8),
            end: Offset(1.0, 1.0),
          ),
          MoveEffect(
            curve: Curves.easeInOut,
            delay: 250.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.0, 40.0),
            end: Offset(0.0, 0.0),
          ),
        ],
      ),
    });
  }

  @override
  void dispose() {
    _model.dispose();

    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      key: scaffoldKey,
      backgroundColor: FlutterFlowTheme.of(context).secondaryBackground,
      body: SafeArea(
        top: true,
        child: Column(
          mainAxisSize: MainAxisSize.max,
          children: [
            Padding(
              padding: EdgeInsetsDirectional.fromSTEB(20, 12, 20, 16),
              child: Row(
                mainAxisSize: MainAxisSize.max,
                mainAxisAlignment: MainAxisAlignment.end,
                children: [
                  FlutterFlowIconButton(
                    borderColor: FlutterFlowTheme.of(context).alternate,
                    borderRadius: 30,
                    borderWidth: 2,
                    buttonSize: 44,
                    icon: Icon(
                      Icons.close_rounded,
                      color: FlutterFlowTheme.of(context).secondaryText,
                      size: 25,
                    ),
                    onPressed: () async {
                      context.pushNamed(ReservasWidget.routeName);
                    },
                  ),
                ],
              ),
            ),
            Expanded(
              child: Container(
                constraints: BoxConstraints(
                  maxWidth: 530,
                ),
                decoration: BoxDecoration(),
                child: Padding(
                  padding: EdgeInsetsDirectional.fromSTEB(16, 0, 16, 70),
                  child: Column(
                    mainAxisSize: MainAxisSize.max,
                    mainAxisAlignment: MainAxisAlignment.center,
                    children: [
                      Container(
                        width: 140,
                        height: 140,
                        decoration: BoxDecoration(
                          color: FlutterFlowTheme.of(context).accent1,
                          shape: BoxShape.circle,
                          border: Border.all(
                            color: FlutterFlowTheme.of(context).primary,
                            width: 2,
                          ),
                        ),
                        alignment: AlignmentDirectional(0, 0),
                        child: Icon(
                          Icons.check_rounded,
                          color: FlutterFlowTheme.of(context).primary,
                          size: 90,
                        ).animateOnPageLoad(
                            animationsMap['iconOnPageLoadAnimation']!),
                      ).animateOnPageLoad(
                          animationsMap['containerOnPageLoadAnimation']!),
                      Padding(
                        padding: EdgeInsetsDirectional.fromSTEB(0, 24, 0, 0),
                        child: Text(
                          'Reserva efetuada',
                          textAlign: TextAlign.center,
                          style: FlutterFlowTheme.of(context)
                              .displaySmall
                              .override(
                                font: GoogleFonts.interTight(
                                  fontWeight: FlutterFlowTheme.of(context)
                                      .displaySmall
                                      .fontWeight,
                                  fontStyle: FlutterFlowTheme.of(context)
                                      .displaySmall
                                      .fontStyle,
                                ),
                                color: FlutterFlowTheme.of(context).primary,
                                letterSpacing: 0.0,
                                fontWeight: FlutterFlowTheme.of(context)
                                    .displaySmall
                                    .fontWeight,
                                fontStyle: FlutterFlowTheme.of(context)
                                    .displaySmall
                                    .fontStyle,
                              ),
                        ).animateOnPageLoad(
                            animationsMap['textOnPageLoadAnimation1']!),
                      ),
                      Padding(
                        padding: EdgeInsetsDirectional.fromSTEB(0, 24, 0, 0),
                        child: Text(
                          'Com sucesso!',
                          textAlign: TextAlign.center,
                          style: FlutterFlowTheme.of(context)
                              .displayMedium
                              .override(
                                font: GoogleFonts.interTight(
                                  fontWeight: FlutterFlowTheme.of(context)
                                      .displayMedium
                                      .fontWeight,
                                  fontStyle: FlutterFlowTheme.of(context)
                                      .displayMedium
                                      .fontStyle,
                                ),
                                letterSpacing: 0.0,
                                fontWeight: FlutterFlowTheme.of(context)
                                    .displayMedium
                                    .fontWeight,
                                fontStyle: FlutterFlowTheme.of(context)
                                    .displayMedium
                                    .fontStyle,
                              ),
                        ).animateOnPageLoad(
                            animationsMap['textOnPageLoadAnimation2']!),
                      ),
                      Padding(
                        padding: EdgeInsetsDirectional.fromSTEB(12, 8, 12, 24),
                        child: Text(
                          'Seu pagamento está sendo processado, podem levar 1-2 horas para que sua reserva seja confirmada. Aguarde o e-mail de confirmação.',
                          textAlign: TextAlign.center,
                          style:
                              FlutterFlowTheme.of(context).labelLarge.override(
                                    font: GoogleFonts.inter(
                                      fontWeight: FlutterFlowTheme.of(context)
                                          .labelLarge
                                          .fontWeight,
                                      fontStyle: FlutterFlowTheme.of(context)
                                          .labelLarge
                                          .fontStyle,
                                    ),
                                    letterSpacing: 0.0,
                                    fontWeight: FlutterFlowTheme.of(context)
                                        .labelLarge
                                        .fontWeight,
                                    fontStyle: FlutterFlowTheme.of(context)
                                        .labelLarge
                                        .fontStyle,
                                  ),
                        ).animateOnPageLoad(
                            animationsMap['textOnPageLoadAnimation3']!),
                      ),
                      FFButtonWidget(
                        onPressed: () async {
                          context.pushNamed(
                            ReservasWidget.routeName,
                            extra: <String, dynamic>{
                              kTransitionInfoKey: TransitionInfo(
                                hasTransition: true,
                                transitionType: PageTransitionType.bottomToTop,
                                duration: Duration(milliseconds: 300),
                              ),
                            },
                          );
                        },
                        text: 'Ver Reservas',
                        options: FFButtonOptions(
                          width: 230,
                          height: 50,
                          padding: EdgeInsetsDirectional.fromSTEB(0, 0, 0, 0),
                          iconPadding:
                              EdgeInsetsDirectional.fromSTEB(0, 0, 0, 0),
                          color: FlutterFlowTheme.of(context).alternate,
                          textStyle:
                              FlutterFlowTheme.of(context).bodyLarge.override(
                                    font: GoogleFonts.inter(
                                      fontWeight: FlutterFlowTheme.of(context)
                                          .bodyLarge
                                          .fontWeight,
                                      fontStyle: FlutterFlowTheme.of(context)
                                          .bodyLarge
                                          .fontStyle,
                                    ),
                                    letterSpacing: 0.0,
                                    fontWeight: FlutterFlowTheme.of(context)
                                        .bodyLarge
                                        .fontWeight,
                                    fontStyle: FlutterFlowTheme.of(context)
                                        .bodyLarge
                                        .fontStyle,
                                  ),
                          elevation: 0,
                          borderSide: BorderSide(
                            color: Colors.transparent,
                            width: 1,
                          ),
                          borderRadius: BorderRadius.circular(40),
                        ),
                      ).animateOnPageLoad(
                          animationsMap['buttonOnPageLoadAnimation']!),
                    ],
                  ),
                ),
              ),
            ),
          ],
        ),
      ),
    );
  }
}
# 7. Código fonte

Disponibilizar o código fonte da aplicação.

import '/backend/backend.dart';
import '/flutter_flow/flutter_flow_animations.dart';
import '/flutter_flow/flutter_flow_icon_button.dart';
import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import '/flutter_flow/flutter_flow_widgets.dart';
import 'dart:math';
import 'dart:ui';
import '/index.dart';
import 'package:smooth_page_indicator/smooth_page_indicator.dart'
    as smooth_page_indicator;
import 'package:cloud_firestore/cloud_firestore.dart';
import 'package:flutter/material.dart';
import 'package:flutter/scheduler.dart';
import 'package:flutter_animate/flutter_animate.dart';
import 'package:flutter_rating_bar/flutter_rating_bar.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:provider/provider.dart';

import 'detalhes_quarto_model.dart';
export 'detalhes_quarto_model.dart';

class DetalhesQuartoWidget extends StatefulWidget {
  const DetalhesQuartoWidget({
    super.key,
    required this.selectedRoom,
  });

  /// the room selected in the roomselectionpage
  final DocumentReference? selectedRoom;

  static String routeName = 'DetalhesQuarto';
  static String routePath = '/detalhesQuarto';

  @override
  State<DetalhesQuartoWidget> createState() => _DetalhesQuartoWidgetState();
}

class _DetalhesQuartoWidgetState extends State<DetalhesQuartoWidget>
    with TickerProviderStateMixin {
  late DetalhesQuartoModel _model;

  final scaffoldKey = GlobalKey<ScaffoldState>();

  final animationsMap = <String, AnimationInfo>{};

  @override
  void initState() {
    super.initState();
    _model = createModel(context, () => DetalhesQuartoModel());

    animationsMap.addAll({
      'pageViewOnPageLoadAnimation': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 1.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          TiltEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: Offset(-0.349, 0),
            end: Offset(0, 0),
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.9, 0.9),
            end: Offset(1.0, 1.0),
          ),
          MoveEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.0, 100.0),
            end: Offset(0.0, 0.0),
          ),
        ],
      ),
      'blurOnPageLoadAnimation': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 400.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 400.0.ms,
            duration: 500.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          TiltEffect(
            curve: Curves.easeInOut,
            delay: 400.0.ms,
            duration: 500.0.ms,
            begin: Offset(-1.396, 0),
            end: Offset(0, 0),
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 400.0.ms,
            duration: 500.0.ms,
            begin: Offset(0.7, 0.7),
            end: Offset(1.0, 1.0),
          ),
          MoveEffect(
            curve: Curves.easeInOut,
            delay: 400.0.ms,
            duration: 500.0.ms,
            begin: Offset(0.0, 30.0),
            end: Offset(0.0, 0.0),
          ),
        ],
      ),
      'columnOnPageLoadAnimation': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 200.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 500.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          TiltEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 500.0.ms,
            begin: Offset(-1.396, 0),
            end: Offset(0, 0),
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 500.0.ms,
            begin: Offset(0.7, 0.7),
            end: Offset(1.0, 1.0),
          ),
          MoveEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 500.0.ms,
            begin: Offset(0.0, 30.0),
            end: Offset(0.0, 0.0),
          ),
        ],
      ),
    });
  }

  @override
  void dispose() {
    _model.dispose();

    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return FutureBuilder<RoomTypeRecord>(
      future: RoomTypeRecord.getDocumentOnce(widget!.selectedRoom!),
      builder: (context, snapshot) {
        // Customize what your widget looks like when it's loading.
        if (!snapshot.hasData) {
          return Scaffold(
            backgroundColor: Colors.white,
            body: Center(
              child: SizedBox(
                width: 50,
                height: 50,
                child: CircularProgressIndicator(
                  valueColor: AlwaysStoppedAnimation<Color>(
                    FlutterFlowTheme.of(context).primary,
                  ),
                ),
              ),
            ),
          );
        }

        final detalhesQuartoRoomTypeRecord = snapshot.data!;

        return GestureDetector(
          onTap: () {
            FocusScope.of(context).unfocus();
            FocusManager.instance.primaryFocus?.unfocus();
          },
          child: Scaffold(
            key: scaffoldKey,
            backgroundColor: Colors.white,
            appBar: AppBar(
              backgroundColor: Colors.white,
              automaticallyImplyLeading: false,
              leading: FlutterFlowIconButton(
                borderColor: Colors.transparent,
                borderRadius: 30,
                borderWidth: 1,
                buttonSize: 60,
                icon: Icon(
                  Icons.arrow_back_rounded,
                  color: Color(0xFF15161E),
                  size: 30,
                ),
                onPressed: () async {
                  context.pop();
                },
              ),
              actions: [],
              centerTitle: false,
              elevation: 0,
            ),
            body: SingleChildScrollView(
              child: Column(
                mainAxisSize: MainAxisSize.max,
                children: [
                  Align(
                    alignment: AlignmentDirectional(0, 1),
                    child: Container(
                      width: double.infinity,
                      height: 470,
                      child: Stack(
                        alignment: AlignmentDirectional(0, -1),
                        children: [
                          Container(
                            width: double.infinity,
                            height: 470,
                            child: Stack(
                              children: [
                                PageView(
                                  controller: _model.pageViewController ??=
                                      PageController(initialPage: 0),
                                  onPageChanged: (_) => safeSetState(() {}),
                                  scrollDirection: Axis.horizontal,
                                  children: [
                                    ClipRRect(
                                      borderRadius: BorderRadius.circular(0),
                                      child: Image.network(
                                        'https://images.unsplash.com/photo-1502672260266-1c1ef2d93688?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w0NTYyMDF8MHwxfHNlYXJjaHwxfHxhcGFydG1lbnR8ZW58MHx8fHwxNzA2ODIyMDczfDA&ixlib=rb-4.0.3&q=80&w=1080',
                                        width: 300,
                                        height: 200,
                                        fit: BoxFit.cover,
                                      ),
                                    ),
                                    ClipRRect(
                                      borderRadius: BorderRadius.circular(0),
                                      child: Image.network(
                                        'https://images.unsplash.com/photo-1493809842364-78817add7ffb?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w0NTYyMDF8MHwxfHNlYXJjaHw4fHxhcGFydG1lbnR8ZW58MHx8fHwxNzA2ODIyMDczfDA&ixlib=rb-4.0.3&q=80&w=1080',
                                        width: 300,
                                        height: 200,
                                        fit: BoxFit.cover,
                                      ),
                                    ),
                                    ClipRRect(
                                      borderRadius: BorderRadius.circular(0),
                                      child: Image.network(
                                        'https://images.unsplash.com/photo-1545324418-cc1a3fa10c00?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w0NTYyMDF8MHwxfHNlYXJjaHw2fHxhcGFydG1lbnR8ZW58MHx8fHwxNzA2ODIyMDczfDA&ixlib=rb-4.0.3&q=80&w=1080',
                                        width: 300,
                                        height: 200,
                                        fit: BoxFit.cover,
                                      ),
                                    ),
                                  ],
                                ),
                                Align(
                                  alignment: AlignmentDirectional(0, 0.75),
                                  child: Padding(
                                    padding: EdgeInsetsDirectional.fromSTEB(
                                        16, 0, 16, 16),
                                    child: smooth_page_indicator
                                        .SmoothPageIndicator(
                                      controller: _model.pageViewController ??=
                                          PageController(initialPage: 0),
                                      count: 3,
                                      axisDirection: Axis.horizontal,
                                      onDotClicked: (i) async {
                                        await _model.pageViewController!
                                            .animateToPage(
                                          i,
                                          duration: Duration(milliseconds: 500),
                                          curve: Curves.ease,
                                        );
                                        safeSetState(() {});
                                      },
                                      effect: smooth_page_indicator
                                          .ExpandingDotsEffect(
                                        expansionFactor: 3,
                                        spacing: 8,
                                        radius: 16,
                                        dotWidth: 16,
                                        dotHeight: 8,
                                        dotColor: Color(0x9AFFFFFF),
                                        activeDotColor: Colors.white,
                                        paintStyle: PaintingStyle.fill,
                                      ),
                                    ),
                                  ),
                                ),
                              ],
                            ),
                          ).animateOnPageLoad(
                              animationsMap['pageViewOnPageLoadAnimation']!),
                          Align(
                            alignment: AlignmentDirectional(0, 1),
                            child: Padding(
                              padding: EdgeInsetsDirectional.fromSTEB(
                                  16, 12, 16, 12),
                              child: ClipRRect(
                                borderRadius: BorderRadius.circular(12),
                                child: BackdropFilter(
                                  filter: ImageFilter.blur(
                                    sigmaX: 7,
                                    sigmaY: 2,
                                  ),
                                  child: Container(
                                    width: double.infinity,
                                    height: 50,
                                    constraints: BoxConstraints(
                                      maxWidth: 870,
                                    ),
                                    decoration: BoxDecoration(
                                      color: Color(0x9AFFFFFF),
                                      borderRadius: BorderRadius.circular(12),
                                      border: Border.all(
                                        color: Color(0x9AFFFFFF),
                                        width: 1,
                                      ),
                                    ),
                                    child: Padding(
                                      padding: EdgeInsetsDirectional.fromSTEB(
                                          16, 0, 16, 0),
                                      child: Row(
                                        mainAxisSize: MainAxisSize.max,
                                        children: [
                                          Expanded(
                                            child: Row(
                                              mainAxisSize: MainAxisSize.max,
                                              mainAxisAlignment:
                                                  MainAxisAlignment.center,
                                              children: [
                                                Icon(
                                                  Icons.bed_rounded,
                                                  color: Color(0xFF15161E),
                                                  size: 24,
                                                ),
                                                Text(
                                                  valueOrDefault<String>(
                                                    detalhesQuartoRoomTypeRecord
                                                        .hospedes
                                                        .toString(),
                                                    '2',
                                                  ),
                                                  style: FlutterFlowTheme.of(
                                                          context)
                                                      .bodyMedium
                                                      .override(
                                                        font:
                                                            GoogleFonts.figtree(
                                                          fontWeight:
                                                              FontWeight.w600,
                                                          fontStyle:
                                                              FlutterFlowTheme.of(
                                                                      context)
                                                                  .bodyMedium
                                                                  .fontStyle,
                                                        ),
                                                        color:
                                                            Color(0xFF15161E),
                                                        fontSize: 14,
                                                        letterSpacing: 0.0,
                                                        fontWeight:
                                                            FontWeight.w600,
                                                        fontStyle:
                                                            FlutterFlowTheme.of(
                                                                    context)
                                                                .bodyMedium
                                                                .fontStyle,
                                                      ),
                                                ),
                                                Text(
                                                  'Hóspedes',
                                                  style: FlutterFlowTheme.of(
                                                          context)
                                                      .bodyMedium
                                                      .override(
                                                        font: GoogleFonts.inter(
                                                          fontWeight:
                                                              FlutterFlowTheme.of(
                                                                      context)
                                                                  .bodyMedium
                                                                  .fontWeight,
                                                          fontStyle:
                                                              FlutterFlowTheme.of(
                                                                      context)
                                                                  .bodyMedium
                                                                  .fontStyle,
                                                        ),
                                                        letterSpacing: 0.0,
                                                        fontWeight:
                                                            FlutterFlowTheme.of(
                                                                    context)
                                                                .bodyMedium
                                                                .fontWeight,
                                                        fontStyle:
                                                            FlutterFlowTheme.of(
                                                                    context)
                                                                .bodyMedium
                                                                .fontStyle,
                                                      ),
                                                ),
                                              ].divide(SizedBox(width: 4)),
                                            ),
                                          ),
                                          Expanded(
                                            child: Row(
                                              mainAxisSize: MainAxisSize.max,
                                              mainAxisAlignment:
                                                  MainAxisAlignment.center,
                                              children: [
                                                Icon(
                                                  Icons.bathtub_outlined,
                                                  color: Color(0xFF15161E),
                                                  size: 24,
                                                ),
                                                Text(
                                                  valueOrDefault<String>(
                                                    detalhesQuartoRoomTypeRecord
                                                        .banheiros
                                                        .toString(),
                                                    '1',
                                                  ),
                                                  style: FlutterFlowTheme.of(
                                                          context)
                                                      .bodyMedium
                                                      .override(
                                                        font:
                                                            GoogleFonts.figtree(
                                                          fontWeight:
                                                              FontWeight.w600,
                                                          fontStyle:
                                                              FlutterFlowTheme.of(
                                                                      context)
                                                                  .bodyMedium
                                                                  .fontStyle,
                                                        ),
                                                        color:
                                                            Color(0xFF15161E),
                                                        fontSize: 14,
                                                        letterSpacing: 0.0,
                                                        fontWeight:
                                                            FontWeight.w600,
                                                        fontStyle:
                                                            FlutterFlowTheme.of(
                                                                    context)
                                                                .bodyMedium
                                                                .fontStyle,
                                                      ),
                                                ),
                                                Text(
                                                  'Banheiro(s)',
                                                  style: FlutterFlowTheme.of(
                                                          context)
                                                      .bodyMedium
                                                      .override(
                                                        font: GoogleFonts.inter(
                                                          fontWeight:
                                                              FlutterFlowTheme.of(
                                                                      context)
                                                                  .bodyMedium
                                                                  .fontWeight,
                                                          fontStyle:
                                                              FlutterFlowTheme.of(
                                                                      context)
                                                                  .bodyMedium
                                                                  .fontStyle,
                                                        ),
                                                        letterSpacing: 0.0,
                                                        fontWeight:
                                                            FlutterFlowTheme.of(
                                                                    context)
                                                                .bodyMedium
                                                                .fontWeight,
                                                        fontStyle:
                                                            FlutterFlowTheme.of(
                                                                    context)
                                                                .bodyMedium
                                                                .fontStyle,
                                                      ),
                                                ),
                                              ].divide(SizedBox(width: 4)),
                                            ),
                                          ),
                                          Expanded(
                                            child: Row(
                                              mainAxisSize: MainAxisSize.max,
                                              mainAxisAlignment:
                                                  MainAxisAlignment.center,
                                              children: [
                                                RatingBar.builder(
                                                  onRatingUpdate: (newValue) =>
                                                      safeSetState(() => _model
                                                              .ratingBarValue =
                                                          newValue),
                                                  itemBuilder:
                                                      (context, index) => Icon(
                                                    Icons.star_rounded,
                                                    color: FlutterFlowTheme.of(
                                                            context)
                                                        .warning,
                                                  ),
                                                  direction: Axis.horizontal,
                                                  initialRating: _model
                                                          .ratingBarValue ??=
                                                      valueOrDefault<double>(
                                                    detalhesQuartoRoomTypeRecord
                                                        .banheiros
                                                        .toDouble(),
                                                    1.0,
                                                  ),
                                                  unratedColor:
                                                      FlutterFlowTheme.of(
                                                              context)
                                                          .alternate,
                                                  itemCount: 5,
                                                  itemSize: 24,
                                                  glowColor:
                                                      FlutterFlowTheme.of(
                                                              context)
                                                          .warning,
                                                ),
                                              ].divide(SizedBox(width: 4)),
                                            ),
                                          ),
                                        ].divide(SizedBox(width: 4)),
                                      ),
                                    ),
                                  ),
                                ),
                              ).animateOnPageLoad(
                                  animationsMap['blurOnPageLoadAnimation']!),
                            ),
                          ),
                        ],
                      ),
                    ),
                  ),
                  Container(
                    constraints: BoxConstraints(
                      maxWidth: 870,
                    ),
                    decoration: BoxDecoration(),
                    child: Stack(
                      children: [
                        Align(
                          alignment: AlignmentDirectional(0, 0),
                          child: Padding(
                            padding: EdgeInsets.all(16),
                            child: Column(
                              mainAxisSize: MainAxisSize.max,
                              crossAxisAlignment: CrossAxisAlignment.start,
                              children: [
                                Row(
                                  mainAxisSize: MainAxisSize.max,
                                  mainAxisAlignment:
                                      MainAxisAlignment.spaceBetween,
                                  children: [
                                    Text(
                                      valueOrDefault<String>(
                                        detalhesQuartoRoomTypeRecord.nome,
                                        'Suite Premium Casal',
                                      ),
                                      style: FlutterFlowTheme.of(context)
                                          .headlineMedium
                                          .override(
                                            font: GoogleFonts.outfit(
                                              fontWeight: FontWeight.w500,
                                              fontStyle:
                                                  FlutterFlowTheme.of(context)
                                                      .headlineMedium
                                                      .fontStyle,
                                            ),
                                            color: Color(0xFF15161E),
                                            fontSize: 24,
                                            letterSpacing: 0.0,
                                            fontWeight: FontWeight.w500,
                                            fontStyle:
                                                FlutterFlowTheme.of(context)
                                                    .headlineMedium
                                                    .fontStyle,
                                          ),
                                    ),
                                    Container(
                                      height: 32,
                                      decoration: BoxDecoration(
                                        color: Color(0x4C39D2C0),
                                        borderRadius: BorderRadius.circular(12),
                                        border: Border.all(
                                          color: Color(0xFF39D2C0),
                                          width: 2,
                                        ),
                                      ),
                                      child: Align(
                                        alignment: AlignmentDirectional(0, 0),
                                        child: Padding(
                                          padding:
                                              EdgeInsetsDirectional.fromSTEB(
                                                  12, 0, 12, 0),
                                          child: Text(
                                            'Disponível - Faça uma reserva',
                                            style: FlutterFlowTheme.of(context)
                                                .bodyMedium
                                                .override(
                                                  font: GoogleFonts.figtree(
                                                    fontWeight: FontWeight.w600,
                                                    fontStyle:
                                                        FlutterFlowTheme.of(
                                                                context)
                                                            .bodyMedium
                                                            .fontStyle,
                                                  ),
                                                  color: Color(0xFF15161E),
                                                  fontSize: 14,
                                                  letterSpacing: 0.0,
                                                  fontWeight: FontWeight.w600,
                                                  fontStyle:
                                                      FlutterFlowTheme.of(
                                                              context)
                                                          .bodyMedium
                                                          .fontStyle,
                                                ),
                                          ),
                                        ),
                                      ),
                                    ),
                                  ].divide(SizedBox(width: 8)),
                                ),
                                Divider(
                                  height: 16,
                                  thickness: 1,
                                  color: Color(0xFFE5E7EB),
                                ),
                                Text(
                                  'Valor',
                                  style: FlutterFlowTheme.of(context)
                                      .labelMedium
                                      .override(
                                        font: GoogleFonts.outfit(
                                          fontWeight: FontWeight.w500,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .labelMedium
                                                  .fontStyle,
                                        ),
                                        color: Color(0xFF606A85),
                                        fontSize: 14,
                                        letterSpacing: 0.0,
                                        fontWeight: FontWeight.w500,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .labelMedium
                                            .fontStyle,
                                      ),
                                ),
                                Row(
                                  mainAxisSize: MainAxisSize.max,
                                  mainAxisAlignment:
                                      MainAxisAlignment.spaceBetween,
                                  children: [
                                    Row(
                                      mainAxisSize: MainAxisSize.max,
                                      children: [
                                        Text(
                                          valueOrDefault<String>(
                                            formatNumber(
                                              detalhesQuartoRoomTypeRecord
                                                  .valordiaria,
                                              formatType: FormatType.decimal,
                                              decimalType:
                                                  DecimalType.automatic,
                                              currency: 'R\$',
                                            ),
                                            'R\$450,00',
                                          ),
                                          style: FlutterFlowTheme.of(context)
                                              .bodyLarge
                                              .override(
                                                font: GoogleFonts.figtree(
                                                  fontWeight: FontWeight.w600,
                                                  fontStyle:
                                                      FlutterFlowTheme.of(
                                                              context)
                                                          .bodyLarge
                                                          .fontStyle,
                                                ),
                                                color: Color(0xFF15161E),
                                                fontSize: 16,
                                                letterSpacing: 0.0,
                                                fontWeight: FontWeight.w600,
                                                fontStyle:
                                                    FlutterFlowTheme.of(context)
                                                        .bodyLarge
                                                        .fontStyle,
                                              ),
                                        ),
                                        Text(
                                          'por dia',
                                          style: FlutterFlowTheme.of(context)
                                              .labelMedium
                                              .override(
                                                font: GoogleFonts.outfit(
                                                  fontWeight: FontWeight.w500,
                                                  fontStyle:
                                                      FlutterFlowTheme.of(
                                                              context)
                                                          .labelMedium
                                                          .fontStyle,
                                                ),
                                                color: Color(0xFF606A85),
                                                fontSize: 14,
                                                letterSpacing: 0.0,
                                                fontWeight: FontWeight.w500,
                                                fontStyle:
                                                    FlutterFlowTheme.of(context)
                                                        .labelMedium
                                                        .fontStyle,
                                              ),
                                        ),
                                      ].divide(SizedBox(width: 4)),
                                    ),
                                    FFButtonWidget(
                                      onPressed: () async {
                                        FFAppState().addToMyReservation(
                                            detalhesQuartoRoomTypeRecord
                                                .reference);
                                        FFAppState().addToMyCartSummary(
                                            detalhesQuartoRoomTypeRecord
                                                .valordiaria);
                                        safeSetState(() {});
                                        ScaffoldMessenger.of(context)
                                            .showSnackBar(
                                          SnackBar(
                                            content: Text(
                                              'Você adicionou esta seleçâo à sua reserva',
                                              style: TextStyle(
                                                color:
                                                    FlutterFlowTheme.of(context)
                                                        .primaryText,
                                              ),
                                            ),
                                            duration:
                                                Duration(milliseconds: 4000),
                                            backgroundColor:
                                                FlutterFlowTheme.of(context)
                                                    .secondary,
                                          ),
                                        );

                                        context.pushNamed(
                                            DetalhesReservasWidget.routeName);
                                      },
                                      text: 'Reserve já!',
                                      options: FFButtonOptions(
                                        height: 40,
                                        padding: EdgeInsetsDirectional.fromSTEB(
                                            16, 0, 16, 0),
                                        iconPadding:
                                            EdgeInsetsDirectional.fromSTEB(
                                                0, 0, 0, 0),
                                        color: FlutterFlowTheme.of(context)
                                            .secondary,
                                        textStyle: FlutterFlowTheme.of(context)
                                            .titleSmall
                                            .override(
                                              font: GoogleFonts.interTight(
                                                fontWeight:
                                                    FlutterFlowTheme.of(context)
                                                        .titleSmall
                                                        .fontWeight,
                                                fontStyle:
                                                    FlutterFlowTheme.of(context)
                                                        .titleSmall
                                                        .fontStyle,
                                              ),
                                              color: Colors.white,
                                              letterSpacing: 0.0,
                                              fontWeight:
                                                  FlutterFlowTheme.of(context)
                                                      .titleSmall
                                                      .fontWeight,
                                              fontStyle:
                                                  FlutterFlowTheme.of(context)
                                                      .titleSmall
                                                      .fontStyle,
                                            ),
                                        elevation: 0,
                                        borderRadius: BorderRadius.circular(8),
                                      ),
                                    ),
                                  ],
                                ),
                                Divider(
                                  height: 16,
                                  thickness: 1,
                                  color: Color(0xFFE5E7EB),
                                ),
                                Text(
                                  'Amenidades',
                                  style: FlutterFlowTheme.of(context)
                                      .labelMedium
                                      .override(
                                        font: GoogleFonts.outfit(
                                          fontWeight: FontWeight.w500,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .labelMedium
                                                  .fontStyle,
                                        ),
                                        color: Color(0xFF606A85),
                                        fontSize: 14,
                                        letterSpacing: 0.0,
                                        fontWeight: FontWeight.w500,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .labelMedium
                                            .fontStyle,
                                      ),
                                ),
                                Padding(
                                  padding: EdgeInsetsDirectional.fromSTEB(
                                      0, 0, 0, 1),
                                  child: Container(
                                    width: double.infinity,
                                    height: 60,
                                    decoration: BoxDecoration(
                                      color: Colors.white,
                                    ),
                                    child: Padding(
                                      padding: EdgeInsetsDirectional.fromSTEB(
                                          0, 4, 0, 4),
                                      child: Row(
                                        mainAxisSize: MainAxisSize.max,
                                        children: [
                                          if (detalhesQuartoRoomTypeRecord
                                              .amenidades.isNotEmpty)
                                            Expanded(
                                              child: GridView(
                                                padding: EdgeInsets.zero,
                                                gridDelegate:
                                                    SliverGridDelegateWithFixedCrossAxisCount(
                                                  crossAxisCount: 3,
                                                  crossAxisSpacing: 10,
                                                  mainAxisSpacing: 10,
                                                  childAspectRatio: 1,
                                                ),
                                                scrollDirection: Axis.vertical,
                                                children: [],
                                              ),
                                            ),
                                        ].divide(SizedBox(width: 12)),
                                      ),
                                    ),
                                  ),
                                ),
                                Divider(
                                  height: 16,
                                  thickness: 1,
                                  color: Color(0xFFE5E7EB),
                                ),
                                Text(
                                  'Descrição',
                                  style: FlutterFlowTheme.of(context)
                                      .labelMedium
                                      .override(
                                        font: GoogleFonts.outfit(
                                          fontWeight: FontWeight.w500,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .labelMedium
                                                  .fontStyle,
                                        ),
                                        color: Color(0xFF606A85),
                                        fontSize: 14,
                                        letterSpacing: 0.0,
                                        fontWeight: FontWeight.w500,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .labelMedium
                                            .fontStyle,
                                      ),
                                ),
                                Text(
                                  valueOrDefault<String>(
                                    detalhesQuartoRoomTypeRecord.descricao,
                                    'Lorem ipsum dolor sit amet',
                                  ),
                                  style: FlutterFlowTheme.of(context)
                                      .bodyMedium
                                      .override(
                                        font: GoogleFonts.figtree(
                                          fontWeight: FontWeight.w600,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .bodyMedium
                                                  .fontStyle,
                                        ),
                                        color: Color(0xFF15161E),
                                        fontSize: 14,
                                        letterSpacing: 0.0,
                                        fontWeight: FontWeight.w600,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .bodyMedium
                                            .fontStyle,
                                      ),
                                ),
                                Divider(
                                  height: 16,
                                  thickness: 1,
                                  color: Color(0xFFE5E7EB),
                                ),
                              ].divide(SizedBox(height: 4)),
                            ).animateOnPageLoad(
                                animationsMap['columnOnPageLoadAnimation']!),
                          ),
                        ),
                      ],
                    ),
                  ),
                ].addToEnd(SizedBox(height: 56)),
              ),
            ),
          ),
        );
      },
    );
  }
}


import '/auth/firebase_auth/auth_util.dart';
import '/flutter_flow/flutter_flow_animations.dart';
import '/flutter_flow/flutter_flow_icon_button.dart';
import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import '/flutter_flow/flutter_flow_widgets.dart';
import 'dart:math';
import 'dart:ui';
import '/index.dart';
import 'package:flutter/material.dart';
import 'package:flutter/scheduler.dart';
import 'package:flutter_animate/flutter_animate.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:provider/provider.dart';

import 'auth2_forgot_password_model.dart';
export 'auth2_forgot_password_model.dart';

class Auth2ForgotPasswordWidget extends StatefulWidget {
  const Auth2ForgotPasswordWidget({super.key});

  static String routeName = 'auth_2_ForgotPassword';
  static String routePath = '/auth2ForgotPassword';

  @override
  State<Auth2ForgotPasswordWidget> createState() =>
      _Auth2ForgotPasswordWidgetState();
}

class _Auth2ForgotPasswordWidgetState extends State<Auth2ForgotPasswordWidget>
    with TickerProviderStateMixin {
  late Auth2ForgotPasswordModel _model;

  final scaffoldKey = GlobalKey<ScaffoldState>();

  final animationsMap = <String, AnimationInfo>{};

  @override
  void initState() {
    super.initState();
    _model = createModel(context, () => Auth2ForgotPasswordModel());

    _model.emailAddressTextController ??= TextEditingController();
    _model.emailAddressFocusNode ??= FocusNode();

    animationsMap.addAll({
      'containerOnPageLoadAnimation': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 1.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          MoveEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.0, 140.0),
            end: Offset(0.0, 0.0),
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.9, 0.9),
            end: Offset(1.0, 1.0),
          ),
          TiltEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: Offset(-0.349, 0),
            end: Offset(0, 0),
          ),
        ],
      ),
    });
  }

  @override
  void dispose() {
    _model.dispose();

    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return GestureDetector(
      onTap: () {
        FocusScope.of(context).unfocus();
        FocusManager.instance.primaryFocus?.unfocus();
      },
      child: Scaffold(
        key: scaffoldKey,
        backgroundColor: FlutterFlowTheme.of(context).secondaryBackground,
        body: Container(
          height: double.infinity,
          decoration: BoxDecoration(
            gradient: LinearGradient(
              colors: [
                FlutterFlowTheme.of(context).primary,
                FlutterFlowTheme.of(context).tertiary
              ],
              stops: [0, 1],
              begin: AlignmentDirectional(0.87, -1),
              end: AlignmentDirectional(-0.87, 1),
            ),
          ),
          alignment: AlignmentDirectional(0, -1),
          child: SingleChildScrollView(
            child: Column(
              mainAxisSize: MainAxisSize.max,
              mainAxisAlignment: MainAxisAlignment.center,
              children: [
                Padding(
                  padding: EdgeInsetsDirectional.fromSTEB(0, 70, 0, 32),
                  child: Container(
                    width: 200,
                    height: 70,
                    decoration: BoxDecoration(
                      borderRadius: BorderRadius.circular(16),
                    ),
                    alignment: AlignmentDirectional(0, 0),
                  ),
                ),
                Padding(
                  padding: EdgeInsets.all(16),
                  child: Container(
                    width: double.infinity,
                    constraints: BoxConstraints(
                      maxWidth: 570,
                    ),
                    decoration: BoxDecoration(
                      color: FlutterFlowTheme.of(context).secondaryBackground,
                      boxShadow: [
                        BoxShadow(
                          blurRadius: 4,
                          color: Color(0x33000000),
                          offset: Offset(
                            0,
                            2,
                          ),
                        )
                      ],
                      borderRadius: BorderRadius.circular(12),
                    ),
                    child: Align(
                      alignment: AlignmentDirectional(0, 0),
                      child: Padding(
                        padding: EdgeInsetsDirectional.fromSTEB(32, 20, 32, 32),
                        child: Column(
                          mainAxisSize: MainAxisSize.max,
                          crossAxisAlignment: CrossAxisAlignment.start,
                          children: [
                            Row(
                              mainAxisSize: MainAxisSize.max,
                              children: [
                                FlutterFlowIconButton(
                                  borderColor: FlutterFlowTheme.of(context)
                                      .secondaryBackground,
                                  borderRadius: 12,
                                  borderWidth: 1,
                                  buttonSize: 40,
                                  fillColor: FlutterFlowTheme.of(context)
                                      .secondaryBackground,
                                  icon: Icon(
                                    Icons.arrow_back_rounded,
                                    color: FlutterFlowTheme.of(context)
                                        .primaryText,
                                    size: 24,
                                  ),
                                  onPressed: () async {
                                    context.safePop();
                                  },
                                ),
                              ].divide(SizedBox(width: 12)),
                            ),
                            Padding(
                              padding:
                                  EdgeInsetsDirectional.fromSTEB(0, 12, 0, 0),
                              child: Text(
                                'Forgot Password',
                                textAlign: TextAlign.center,
                                style: FlutterFlowTheme.of(context)
                                    .displaySmall
                                    .override(
                                      font: GoogleFonts.interTight(
                                        fontWeight: FlutterFlowTheme.of(context)
                                            .displaySmall
                                            .fontWeight,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .displaySmall
                                            .fontStyle,
                                      ),
                                      letterSpacing: 0.0,
                                      fontWeight: FlutterFlowTheme.of(context)
                                          .displaySmall
                                          .fontWeight,
                                      fontStyle: FlutterFlowTheme.of(context)
                                          .displaySmall
                                          .fontStyle,
                                    ),
                              ),
                            ),
                            Padding(
                              padding:
                                  EdgeInsetsDirectional.fromSTEB(0, 8, 0, 24),
                              child: Text(
                                'Please fill out your email belo in order to recieve a reset password link.',
                                textAlign: TextAlign.start,
                                style: FlutterFlowTheme.of(context)
                                    .labelLarge
                                    .override(
                                      font: GoogleFonts.inter(
                                        fontWeight: FlutterFlowTheme.of(context)
                                            .labelLarge
                                            .fontWeight,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .labelLarge
                                            .fontStyle,
                                      ),
                                      letterSpacing: 0.0,
                                      fontWeight: FlutterFlowTheme.of(context)
                                          .labelLarge
                                          .fontWeight,
                                      fontStyle: FlutterFlowTheme.of(context)
                                          .labelLarge
                                          .fontStyle,
                                    ),
                              ),
                            ),
                            Padding(
                              padding:
                                  EdgeInsetsDirectional.fromSTEB(0, 0, 0, 16),
                              child: Container(
                                width: double.infinity,
                                child: TextFormField(
                                  controller: _model.emailAddressTextController,
                                  focusNode: _model.emailAddressFocusNode,
                                  autofocus: true,
                                  autofillHints: [AutofillHints.email],
                                  obscureText: false,
                                  decoration: InputDecoration(
                                    labelText: 'Email',
                                    labelStyle: FlutterFlowTheme.of(context)
                                        .labelLarge
                                        .override(
                                          font: GoogleFonts.inter(
                                            fontWeight:
                                                FlutterFlowTheme.of(context)
                                                    .labelLarge
                                                    .fontWeight,
                                            fontStyle:
                                                FlutterFlowTheme.of(context)
                                                    .labelLarge
                                                    .fontStyle,
                                          ),
                                          letterSpacing: 0.0,
                                          fontWeight:
                                              FlutterFlowTheme.of(context)
                                                  .labelLarge
                                                  .fontWeight,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .labelLarge
                                                  .fontStyle,
                                        ),
                                    enabledBorder: OutlineInputBorder(
                                      borderSide: BorderSide(
                                        color: FlutterFlowTheme.of(context)
                                            .alternate,
                                        width: 2,
                                      ),
                                      borderRadius: BorderRadius.circular(12),
                                    ),
                                    focusedBorder: OutlineInputBorder(
                                      borderSide: BorderSide(
                                        color: FlutterFlowTheme.of(context)
                                            .primary,
                                        width: 2,
                                      ),
                                      borderRadius: BorderRadius.circular(12),
                                    ),
                                    errorBorder: OutlineInputBorder(
                                      borderSide: BorderSide(
                                        color:
                                            FlutterFlowTheme.of(context).error,
                                        width: 2,
                                      ),
                                      borderRadius: BorderRadius.circular(12),
                                    ),
                                    focusedErrorBorder: OutlineInputBorder(
                                      borderSide: BorderSide(
                                        color:
                                            FlutterFlowTheme.of(context).error,
                                        width: 2,
                                      ),
                                      borderRadius: BorderRadius.circular(12),
                                    ),
                                    filled: true,
                                    fillColor: FlutterFlowTheme.of(context)
                                        .primaryBackground,
                                  ),
                                  style: FlutterFlowTheme.of(context)
                                      .bodyLarge
                                      .override(
                                        font: GoogleFonts.inter(
                                          fontWeight:
                                              FlutterFlowTheme.of(context)
                                                  .bodyLarge
                                                  .fontWeight,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .bodyLarge
                                                  .fontStyle,
                                        ),
                                        letterSpacing: 0.0,
                                        fontWeight: FlutterFlowTheme.of(context)
                                            .bodyLarge
                                            .fontWeight,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .bodyLarge
                                            .fontStyle,
                                      ),
                                  keyboardType: TextInputType.emailAddress,
                                  cursorColor:
                                      FlutterFlowTheme.of(context).primary,
                                  validator: _model
                                      .emailAddressTextControllerValidator
                                      .asValidator(context),
                                ),
                              ),
                            ),
                            Padding(
                              padding:
                                  EdgeInsetsDirectional.fromSTEB(0, 0, 0, 16),
                              child: FFButtonWidget(
                                onPressed: () async {
                                  if (_model.emailAddressTextController.text
                                      .isEmpty) {
                                    ScaffoldMessenger.of(context).showSnackBar(
                                      SnackBar(
                                        content: Text(
                                          'Email required!',
                                        ),
                                      ),
                                    );
                                    return;
                                  }
                                  await authManager.resetPassword(
                                    email:
                                        _model.emailAddressTextController.text,
                                    context: context,
                                  );
                                },
                                text: 'Send Reset Link',
                                options: FFButtonOptions(
                                  width: double.infinity,
                                  height: 44,
                                  padding: EdgeInsetsDirectional.fromSTEB(
                                      0, 0, 0, 0),
                                  iconPadding: EdgeInsetsDirectional.fromSTEB(
                                      0, 0, 0, 0),
                                  color: FlutterFlowTheme.of(context).primary,
                                  textStyle: FlutterFlowTheme.of(context)
                                      .titleSmall
                                      .override(
                                        font: GoogleFonts.interTight(
                                          fontWeight:
                                              FlutterFlowTheme.of(context)
                                                  .titleSmall
                                                  .fontWeight,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .titleSmall
                                                  .fontStyle,
                                        ),
                                        color: Colors.white,
                                        letterSpacing: 0.0,
                                        fontWeight: FlutterFlowTheme.of(context)
                                            .titleSmall
                                            .fontWeight,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .titleSmall
                                            .fontStyle,
                                      ),
                                  elevation: 3,
                                  borderSide: BorderSide(
                                    color: Colors.transparent,
                                    width: 1,
                                  ),
                                  borderRadius: BorderRadius.circular(12),
                                ),
                              ),
                            ),
                          ],
                        ),
                      ),
                    ),
                  ).animateOnPageLoad(
                      animationsMap['containerOnPageLoadAnimation']!),
                ),
              ],
            ),
          ),
        ),
      ),
    );
  }
}


import '/account_profile_creation/edit_profile_auth_2/edit_profile_auth2_widget.dart';
import '/flutter_flow/flutter_flow_animations.dart';
import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import '/flutter_flow/flutter_flow_widgets.dart';
import 'dart:math';
import 'dart:ui';
import '/index.dart';
import 'package:flutter/material.dart';
import 'package:flutter/scheduler.dart';
import 'package:flutter_animate/flutter_animate.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:provider/provider.dart';

import 'auth2_create_profile_model.dart';
export 'auth2_create_profile_model.dart';

class Auth2CreateProfileWidget extends StatefulWidget {
  const Auth2CreateProfileWidget({super.key});

  static String routeName = 'auth_2_createProfile';
  static String routePath = '/auth2CreateProfile';

  @override
  State<Auth2CreateProfileWidget> createState() =>
      _Auth2CreateProfileWidgetState();
}

class _Auth2CreateProfileWidgetState extends State<Auth2CreateProfileWidget>
    with TickerProviderStateMixin {
  late Auth2CreateProfileModel _model;

  final scaffoldKey = GlobalKey<ScaffoldState>();

  final animationsMap = <String, AnimationInfo>{};

  @override
  void initState() {
    super.initState();
    _model = createModel(context, () => Auth2CreateProfileModel());

    animationsMap.addAll({
      'containerOnPageLoadAnimation': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 1.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          MoveEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.0, 140.0),
            end: Offset(0.0, 0.0),
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: Offset(0.9, 0.9),
            end: Offset(1.0, 1.0),
          ),
          TiltEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 300.0.ms,
            begin: Offset(-0.349, 0),
            end: Offset(0, 0),
          ),
        ],
      ),
    });
  }

  @override
  void dispose() {
    _model.dispose();

    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return GestureDetector(
      onTap: () {
        FocusScope.of(context).unfocus();
        FocusManager.instance.primaryFocus?.unfocus();
      },
      child: Scaffold(
        key: scaffoldKey,
        backgroundColor: FlutterFlowTheme.of(context).secondaryBackground,
        body: Container(
          height: double.infinity,
          decoration: BoxDecoration(
            gradient: LinearGradient(
              colors: [
                FlutterFlowTheme.of(context).primary,
                FlutterFlowTheme.of(context).tertiary
              ],
              stops: [0, 1],
              begin: AlignmentDirectional(0.87, -1),
              end: AlignmentDirectional(-0.87, 1),
            ),
          ),
          alignment: AlignmentDirectional(0, -1),
          child: SingleChildScrollView(
            child: Column(
              mainAxisSize: MainAxisSize.max,
              mainAxisAlignment: MainAxisAlignment.center,
              children: [
                Padding(
                  padding: EdgeInsetsDirectional.fromSTEB(0, 70, 0, 32),
                  child: Container(
                    width: 200,
                    height: 70,
                    decoration: BoxDecoration(
                      borderRadius: BorderRadius.circular(16),
                    ),
                    alignment: AlignmentDirectional(0, 0),
                  ),
                ),
                Padding(
                  padding: EdgeInsets.all(16),
                  child: Container(
                    width: double.infinity,
                    constraints: BoxConstraints(
                      maxWidth: 570,
                    ),
                    decoration: BoxDecoration(
                      color: FlutterFlowTheme.of(context).secondaryBackground,
                      boxShadow: [
                        BoxShadow(
                          blurRadius: 4,
                          color: Color(0x33000000),
                          offset: Offset(
                            0,
                            2,
                          ),
                        )
                      ],
                      borderRadius: BorderRadius.circular(12),
                    ),
                    child: Padding(
                      padding: EdgeInsetsDirectional.fromSTEB(0, 24, 0, 24),
                      child: wrapWithModel(
                        model: _model.editProfileAuth2Model,
                        updateCallback: () => safeSetState(() {}),
                        child: EditProfileAuth2Widget(
                          title: 'Create Profile',
                          confirmButtonText: 'Save & Continue',
                          navigateAction: () async {
                            context.pushNamed(Auth2ProfileWidget.routeName);
                          },
                        ),
                      ),
                    ),
                  ).animateOnPageLoad(
                      animationsMap['containerOnPageLoadAnimation']!),
                ),
              ],
            ),
          ),
        ),
      ),
    );
  }
}


import '/auth/firebase_auth/auth_util.dart';
import '/flutter_flow/flutter_flow_animations.dart';
import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import '/flutter_flow/flutter_flow_widgets.dart';
import 'dart:math';
import 'dart:ui';
import '/index.dart';
import 'package:cached_network_image/cached_network_image.dart';
import 'package:flutter/material.dart';
import 'package:flutter/scheduler.dart';
import 'package:flutter_animate/flutter_animate.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:provider/provider.dart';

import 'auth2_profile_model.dart';
export 'auth2_profile_model.dart';

class Auth2ProfileWidget extends StatefulWidget {
  const Auth2ProfileWidget({super.key});

  static String routeName = 'auth_2_Profile';
  static String routePath = '/auth2Profile';

  @override
  State<Auth2ProfileWidget> createState() => _Auth2ProfileWidgetState();
}

class _Auth2ProfileWidgetState extends State<Auth2ProfileWidget>
    with TickerProviderStateMixin {
  late Auth2ProfileModel _model;

  final scaffoldKey = GlobalKey<ScaffoldState>();

  final animationsMap = <String, AnimationInfo>{};

  @override
  void initState() {
    super.initState();
    _model = createModel(context, () => Auth2ProfileModel());

    animationsMap.addAll({
      'containerOnPageLoadAnimation': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 1.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 400.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 400.0.ms,
            begin: Offset(3.0, 3.0),
            end: Offset(1.0, 1.0),
          ),
        ],
      ),
      'buttonOnPageLoadAnimation': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 400.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 400.0.ms,
            duration: 600.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          MoveEffect(
            curve: Curves.easeInOut,
            delay: 400.0.ms,
            duration: 600.0.ms,
            begin: Offset(0.0, 60.0),
            end: Offset(0.0, 0.0),
          ),
        ],
      ),
    });
  }

  @override
  void dispose() {
    _model.dispose();

    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return GestureDetector(
      onTap: () {
        FocusScope.of(context).unfocus();
        FocusManager.instance.primaryFocus?.unfocus();
      },
      child: Scaffold(
        key: scaffoldKey,
        backgroundColor: FlutterFlowTheme.of(context).secondaryBackground,
        body: Align(
          alignment: AlignmentDirectional(0, -1),
          child: Container(
            width: double.infinity,
            constraints: BoxConstraints(
              maxWidth: 770,
            ),
            decoration: BoxDecoration(
              color: FlutterFlowTheme.of(context).secondaryBackground,
            ),
            child: Column(
              mainAxisSize: MainAxisSize.max,
              crossAxisAlignment: CrossAxisAlignment.start,
              children: [
                Container(
                  height: 180,
                  child: Stack(
                    children: [
                      Padding(
                        padding: EdgeInsetsDirectional.fromSTEB(0, 0, 0, 16),
                        child: Container(
                          width: double.infinity,
                          height: 140,
                          decoration: BoxDecoration(
                            gradient: LinearGradient(
                              colors: [
                                FlutterFlowTheme.of(context).primary,
                                FlutterFlowTheme.of(context).error,
                                FlutterFlowTheme.of(context).tertiary
                              ],
                              stops: [0, 0.5, 1],
                              begin: AlignmentDirectional(-1, -1),
                              end: AlignmentDirectional(1, 1),
                            ),
                          ),
                          child: Container(
                            width: 100,
                            height: 200,
                            decoration: BoxDecoration(
                              gradient: LinearGradient(
                                colors: [
                                  Color(0x00FFFFFF),
                                  FlutterFlowTheme.of(context)
                                      .secondaryBackground
                                ],
                                stops: [0, 1],
                                begin: AlignmentDirectional(0, -1),
                                end: AlignmentDirectional(0, 1),
                              ),
                            ),
                          ),
                        ).animateOnPageLoad(
                            animationsMap['containerOnPageLoadAnimation']!),
                      ),
                      Align(
                        alignment: AlignmentDirectional(-1, 1),
                        child: Padding(
                          padding: EdgeInsetsDirectional.fromSTEB(24, 0, 0, 0),
                          child: Container(
                            width: 90,
                            height: 90,
                            decoration: BoxDecoration(
                              color: FlutterFlowTheme.of(context).accent2,
                              shape: BoxShape.circle,
                              border: Border.all(
                                color: FlutterFlowTheme.of(context).secondary,
                                width: 2,
                              ),
                            ),
                            child: Padding(
                              padding: EdgeInsets.all(4),
                              child: AuthUserStreamWidget(
                                builder: (context) => ClipRRect(
                                  borderRadius: BorderRadius.circular(50),
                                  child: CachedNetworkImage(
                                    fadeInDuration: Duration(milliseconds: 500),
                                    fadeOutDuration:
                                        Duration(milliseconds: 500),
                                    imageUrl: currentUserPhoto,
                                    width: 100,
                                    height: 100,
                                    fit: BoxFit.cover,
                                  ),
                                ),
                              ),
                            ),
                          ),
                        ),
                      ),
                    ],
                  ),
                ),
                Padding(
                  padding: EdgeInsetsDirectional.fromSTEB(24, 12, 0, 0),
                  child: AuthUserStreamWidget(
                    builder: (context) => Text(
                      currentUserDisplayName,
                      style: FlutterFlowTheme.of(context).displaySmall.override(
                            font: GoogleFonts.interTight(
                              fontWeight: FlutterFlowTheme.of(context)
                                  .displaySmall
                                  .fontWeight,
                              fontStyle: FlutterFlowTheme.of(context)
                                  .displaySmall
                                  .fontStyle,
                            ),
                            letterSpacing: 0.0,
                            fontWeight: FlutterFlowTheme.of(context)
                                .displaySmall
                                .fontWeight,
                            fontStyle: FlutterFlowTheme.of(context)
                                .displaySmall
                                .fontStyle,
                          ),
                    ),
                  ),
                ),
                Padding(
                  padding: EdgeInsetsDirectional.fromSTEB(24, 4, 0, 16),
                  child: Text(
                    valueOrDefault<String>(
                      currentUserEmail,
                      'andrew@domainname.com',
                    ),
                    style: FlutterFlowTheme.of(context).labelLarge.override(
                          font: GoogleFonts.inter(
                            fontWeight: FlutterFlowTheme.of(context)
                                .labelLarge
                                .fontWeight,
                            fontStyle: FlutterFlowTheme.of(context)
                                .labelLarge
                                .fontStyle,
                          ),
                          color: FlutterFlowTheme.of(context).primary,
                          letterSpacing: 0.0,
                          fontWeight: FlutterFlowTheme.of(context)
                              .labelLarge
                              .fontWeight,
                          fontStyle:
                              FlutterFlowTheme.of(context).labelLarge.fontStyle,
                        ),
                  ),
                ),
                Padding(
                  padding: EdgeInsetsDirectional.fromSTEB(24, 4, 0, 0),
                  child: Text(
                    'Your Account',
                    style: FlutterFlowTheme.of(context).labelMedium.override(
                          font: GoogleFonts.inter(
                            fontWeight: FlutterFlowTheme.of(context)
                                .labelMedium
                                .fontWeight,
                            fontStyle: FlutterFlowTheme.of(context)
                                .labelMedium
                                .fontStyle,
                          ),
                          letterSpacing: 0.0,
                          fontWeight: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontWeight,
                          fontStyle: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontStyle,
                        ),
                  ),
                ),
                Padding(
                  padding: EdgeInsetsDirectional.fromSTEB(16, 12, 16, 0),
                  child: InkWell(
                    splashColor: Colors.transparent,
                    focusColor: Colors.transparent,
                    hoverColor: Colors.transparent,
                    highlightColor: Colors.transparent,
                    onTap: () async {
                      context.pushNamed(Auth2EditProfileWidget.routeName);
                    },
                    child: Container(
                      width: double.infinity,
                      height: 60,
                      decoration: BoxDecoration(
                        color: FlutterFlowTheme.of(context).secondaryBackground,
                        boxShadow: [
                          BoxShadow(
                            blurRadius: 3,
                            color: Color(0x33000000),
                            offset: Offset(
                              0,
                              1,
                            ),
                          )
                        ],
                        borderRadius: BorderRadius.circular(8),
                        shape: BoxShape.rectangle,
                        border: Border.all(
                          color: FlutterFlowTheme.of(context).alternate,
                          width: 1,
                        ),
                      ),
                      child: Padding(
                        padding: EdgeInsets.all(12),
                        child: Row(
                          mainAxisSize: MainAxisSize.max,
                          children: [
                            Icon(
                              Icons.account_circle_outlined,
                              color: FlutterFlowTheme.of(context).secondaryText,
                              size: 24,
                            ),
                            Padding(
                              padding:
                                  EdgeInsetsDirectional.fromSTEB(12, 0, 0, 0),
                              child: Text(
                                'Edit Profile',
                                style: FlutterFlowTheme.of(context)
                                    .labelLarge
                                    .override(
                                      font: GoogleFonts.inter(
                                        fontWeight: FlutterFlowTheme.of(context)
                                            .labelLarge
                                            .fontWeight,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .labelLarge
                                            .fontStyle,
                                      ),
                                      letterSpacing: 0.0,
                                      fontWeight: FlutterFlowTheme.of(context)
                                          .labelLarge
                                          .fontWeight,
                                      fontStyle: FlutterFlowTheme.of(context)
                                          .labelLarge
                                          .fontStyle,
                                    ),
                              ),
                            ),
                            Expanded(
                              child: Align(
                                alignment: AlignmentDirectional(0.9, 0),
                                child: Icon(
                                  Icons.arrow_forward_ios,
                                  color: FlutterFlowTheme.of(context)
                                      .secondaryText,
                                  size: 18,
                                ),
                              ),
                            ),
                          ],
                        ),
                      ),
                    ),
                  ),
                ),
                Padding(
                  padding: EdgeInsetsDirectional.fromSTEB(24, 16, 0, 0),
                  child: Text(
                    'App Settings',
                    style: FlutterFlowTheme.of(context).labelMedium.override(
                          font: GoogleFonts.inter(
                            fontWeight: FlutterFlowTheme.of(context)
                                .labelMedium
                                .fontWeight,
                            fontStyle: FlutterFlowTheme.of(context)
                                .labelMedium
                                .fontStyle,
                          ),
                          letterSpacing: 0.0,
                          fontWeight: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontWeight,
                          fontStyle: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontStyle,
                        ),
                  ),
                ),
                Padding(
                  padding: EdgeInsetsDirectional.fromSTEB(16, 12, 16, 0),
                  child: Container(
                    width: double.infinity,
                    height: 60,
                    decoration: BoxDecoration(
                      color: FlutterFlowTheme.of(context).secondaryBackground,
                      boxShadow: [
                        BoxShadow(
                          blurRadius: 3,
                          color: Color(0x33000000),
                          offset: Offset(
                            0,
                            1,
                          ),
                        )
                      ],
                      borderRadius: BorderRadius.circular(8),
                      shape: BoxShape.rectangle,
                      border: Border.all(
                        color: FlutterFlowTheme.of(context).alternate,
                        width: 1,
                      ),
                    ),
                    child: Padding(
                      padding: EdgeInsets.all(12),
                      child: Row(
                        mainAxisSize: MainAxisSize.max,
                        children: [
                          Icon(
                            Icons.help_outline_rounded,
                            color: FlutterFlowTheme.of(context).secondaryText,
                            size: 24,
                          ),
                          Padding(
                            padding:
                                EdgeInsetsDirectional.fromSTEB(12, 0, 0, 0),
                            child: Text(
                              'Support',
                              style: FlutterFlowTheme.of(context)
                                  .labelLarge
                                  .override(
                                    font: GoogleFonts.inter(
                                      fontWeight: FlutterFlowTheme.of(context)
                                          .labelLarge
                                          .fontWeight,
                                      fontStyle: FlutterFlowTheme.of(context)
                                          .labelLarge
                                          .fontStyle,
                                    ),
                                    letterSpacing: 0.0,
                                    fontWeight: FlutterFlowTheme.of(context)
                                        .labelLarge
                                        .fontWeight,
                                    fontStyle: FlutterFlowTheme.of(context)
                                        .labelLarge
                                        .fontStyle,
                                  ),
                            ),
                          ),
                          Expanded(
                            child: Align(
                              alignment: AlignmentDirectional(0.9, 0),
                              child: Icon(
                                Icons.arrow_forward_ios,
                                color:
                                    FlutterFlowTheme.of(context).secondaryText,
                                size: 18,
                              ),
                            ),
                          ),
                        ],
                      ),
                    ),
                  ),
                ),
                Padding(
                  padding: EdgeInsetsDirectional.fromSTEB(16, 12, 16, 0),
                  child: Container(
                    width: double.infinity,
                    height: 60,
                    decoration: BoxDecoration(
                      color: FlutterFlowTheme.of(context).secondaryBackground,
                      boxShadow: [
                        BoxShadow(
                          blurRadius: 3,
                          color: Color(0x33000000),
                          offset: Offset(
                            0,
                            1,
                          ),
                        )
                      ],
                      borderRadius: BorderRadius.circular(8),
                      shape: BoxShape.rectangle,
                      border: Border.all(
                        color: FlutterFlowTheme.of(context).alternate,
                        width: 1,
                      ),
                    ),
                    child: Padding(
                      padding: EdgeInsets.all(12),
                      child: Row(
                        mainAxisSize: MainAxisSize.max,
                        children: [
                          Icon(
                            Icons.privacy_tip_rounded,
                            color: FlutterFlowTheme.of(context).secondaryText,
                            size: 24,
                          ),
                          Padding(
                            padding:
                                EdgeInsetsDirectional.fromSTEB(12, 0, 0, 0),
                            child: Text(
                              'Terms of Service',
                              style: FlutterFlowTheme.of(context)
                                  .labelLarge
                                  .override(
                                    font: GoogleFonts.inter(
                                      fontWeight: FlutterFlowTheme.of(context)
                                          .labelLarge
                                          .fontWeight,
                                      fontStyle: FlutterFlowTheme.of(context)
                                          .labelLarge
                                          .fontStyle,
                                    ),
                                    letterSpacing: 0.0,
                                    fontWeight: FlutterFlowTheme.of(context)
                                        .labelLarge
                                        .fontWeight,
                                    fontStyle: FlutterFlowTheme.of(context)
                                        .labelLarge
                                        .fontStyle,
                                  ),
                            ),
                          ),
                          Expanded(
                            child: Align(
                              alignment: AlignmentDirectional(0.9, 0),
                              child: Icon(
                                Icons.arrow_forward_ios,
                                color:
                                    FlutterFlowTheme.of(context).secondaryText,
                                size: 18,
                              ),
                            ),
                          ),
                        ],
                      ),
                    ),
                  ),
                ),
                Align(
                  alignment: AlignmentDirectional(0, 0),
                  child: Padding(
                    padding: EdgeInsetsDirectional.fromSTEB(0, 16, 0, 0),
                    child: FFButtonWidget(
                      onPressed: () async {
                        GoRouter.of(context).prepareAuthEvent();
                        await authManager.signOut();
                        GoRouter.of(context).clearRedirectLocation();

                        context.goNamedAuth(
                            ListagemDeQuartosWidget.routeName, context.mounted);
                      },
                      text: 'Log Out',
                      options: FFButtonOptions(
                        width: 150,
                        height: 44,
                        padding: EdgeInsetsDirectional.fromSTEB(0, 0, 0, 0),
                        iconPadding: EdgeInsetsDirectional.fromSTEB(0, 0, 0, 0),
                        color: FlutterFlowTheme.of(context).primaryBackground,
                        textStyle:
                            FlutterFlowTheme.of(context).bodyLarge.override(
                                  font: GoogleFonts.inter(
                                    fontWeight: FlutterFlowTheme.of(context)
                                        .bodyLarge
                                        .fontWeight,
                                    fontStyle: FlutterFlowTheme.of(context)
                                        .bodyLarge
                                        .fontStyle,
                                  ),
                                  letterSpacing: 0.0,
                                  fontWeight: FlutterFlowTheme.of(context)
                                      .bodyLarge
                                      .fontWeight,
                                  fontStyle: FlutterFlowTheme.of(context)
                                      .bodyLarge
                                      .fontStyle,
                                ),
                        elevation: 0,
                        borderSide: BorderSide(
                          color: FlutterFlowTheme.of(context).alternate,
                          width: 1,
                        ),
                        borderRadius: BorderRadius.circular(12),
                      ),
                    ).animateOnPageLoad(
                        animationsMap['buttonOnPageLoadAnimation']!),
                  ),
                ),
              ],
            ),
          ),
        ),
      ),
    );
  }
}


import '/account_profile_creation/edit_profile_auth_2/edit_profile_auth2_widget.dart';
import '/flutter_flow/flutter_flow_animations.dart';
import '/flutter_flow/flutter_flow_icon_button.dart';
import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import '/flutter_flow/flutter_flow_widgets.dart';
import 'dart:math';
import 'dart:ui';
import 'package:flutter/material.dart';
import 'package:flutter/scheduler.dart';
import 'package:flutter_animate/flutter_animate.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:provider/provider.dart';

import 'auth2_edit_profile_model.dart';
export 'auth2_edit_profile_model.dart';

class Auth2EditProfileWidget extends StatefulWidget {
  const Auth2EditProfileWidget({super.key});

  static String routeName = 'auth_2_EditProfile';
  static String routePath = '/auth2EditProfile';

  @override
  State<Auth2EditProfileWidget> createState() => _Auth2EditProfileWidgetState();
}

class _Auth2EditProfileWidgetState extends State<Auth2EditProfileWidget>
    with TickerProviderStateMixin {
  late Auth2EditProfileModel _model;

  final scaffoldKey = GlobalKey<ScaffoldState>();

  final animationsMap = <String, AnimationInfo>{};

  @override
  void initState() {
    super.initState();
    _model = createModel(context, () => Auth2EditProfileModel());

    animationsMap.addAll({
      'containerOnPageLoadAnimation': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 1.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 400.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 0.0.ms,
            duration: 400.0.ms,
            begin: Offset(3.0, 3.0),
            end: Offset(1.0, 1.0),
          ),
        ],
      ),
    });
  }

  @override
  void dispose() {
    _model.dispose();

    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return GestureDetector(
      onTap: () {
        FocusScope.of(context).unfocus();
        FocusManager.instance.primaryFocus?.unfocus();
      },
      child: Scaffold(
        key: scaffoldKey,
        backgroundColor: FlutterFlowTheme.of(context).secondaryBackground,
        body: Column(
          mainAxisSize: MainAxisSize.max,
          mainAxisAlignment: MainAxisAlignment.start,
          children: [
            Padding(
              padding: EdgeInsetsDirectional.fromSTEB(0, 0, 0, 16),
              child: Container(
                width: double.infinity,
                height: 130,
                decoration: BoxDecoration(
                  gradient: LinearGradient(
                    colors: [
                      FlutterFlowTheme.of(context).primary,
                      FlutterFlowTheme.of(context).error,
                      FlutterFlowTheme.of(context).tertiary
                    ],
                    stops: [0, 0.5, 1],
                    begin: AlignmentDirectional(-1, -1),
                    end: AlignmentDirectional(1, 1),
                  ),
                ),
                child: Container(
                  width: 100,
                  height: 200,
                  decoration: BoxDecoration(
                    gradient: LinearGradient(
                      colors: [
                        Color(0x00FFFFFF),
                        FlutterFlowTheme.of(context).secondaryBackground
                      ],
                      stops: [0, 1],
                      begin: AlignmentDirectional(0, -1),
                      end: AlignmentDirectional(0, 1),
                    ),
                  ),
                  child: Align(
                    alignment: AlignmentDirectional(-1, 1),
                    child: Padding(
                      padding: EdgeInsetsDirectional.fromSTEB(16, 0, 0, 24),
                      child: FlutterFlowIconButton(
                        borderColor: FlutterFlowTheme.of(context).accent4,
                        borderRadius: 12,
                        borderWidth: 1,
                        buttonSize: 40,
                        fillColor: FlutterFlowTheme.of(context).accent4,
                        icon: Icon(
                          Icons.arrow_back_rounded,
                          color: FlutterFlowTheme.of(context).primaryText,
                          size: 24,
                        ),
                        onPressed: () async {
                          context.safePop();
                        },
                      ),
                    ),
                  ),
                ),
              ).animateOnPageLoad(
                  animationsMap['containerOnPageLoadAnimation']!),
            ),
            Align(
              alignment: AlignmentDirectional(0, -1),
              child: Container(
                width: double.infinity,
                constraints: BoxConstraints(
                  maxWidth: 770,
                ),
                decoration: BoxDecoration(
                  color: FlutterFlowTheme.of(context).secondaryBackground,
                ),
                child: wrapWithModel(
                  model: _model.editProfileAuth2Model,
                  updateCallback: () => safeSetState(() {}),
                  child: EditProfileAuth2Widget(
                    title: 'Edit Profile',
                    confirmButtonText: 'Save Changes',
                    navigateAction: () async {
                      context.safePop();
                    },
                  ),
                ),
              ),
            ),
          ],
        ),
      ),
    );
  }
}



import '/flutter_flow/flutter_flow_icon_button.dart';
import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import '/flutter_flow/flutter_flow_widgets.dart';
import 'dart:ui';
import 'package:easy_debounce/easy_debounce.dart';
import 'package:flutter/material.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:provider/provider.dart';

import 'listadeusuarios_model.dart';
export 'listadeusuarios_model.dart';

class ListadeusuariosWidget extends StatefulWidget {
  const ListadeusuariosWidget({super.key});

  static String routeName = 'Listadeusuarios';
  static String routePath = '/listadeusuarios';

  @override
  State<ListadeusuariosWidget> createState() => _ListadeusuariosWidgetState();
}

class _ListadeusuariosWidgetState extends State<ListadeusuariosWidget> {
  late ListadeusuariosModel _model;

  final scaffoldKey = GlobalKey<ScaffoldState>();

  @override
  void initState() {
    super.initState();
    _model = createModel(context, () => ListadeusuariosModel());

    _model.textController ??= TextEditingController();
    _model.textFieldFocusNode ??= FocusNode();
  }

  @override
  void dispose() {
    _model.dispose();

    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return GestureDetector(
      onTap: () {
        FocusScope.of(context).unfocus();
        FocusManager.instance.primaryFocus?.unfocus();
      },
      child: Scaffold(
        key: scaffoldKey,
        backgroundColor: Color(0xFFF1F4F8),
        appBar: AppBar(
          backgroundColor: Color(0xFF44BB33),
          automaticallyImplyLeading: false,
          leading: FlutterFlowIconButton(
            borderColor: Colors.transparent,
            borderRadius: 30,
            borderWidth: 1,
            buttonSize: 54,
            icon: Icon(
              Icons.arrow_back_rounded,
              color: Color(0xFF57636C),
              size: 24,
            ),
            onPressed: () {
              print('IconButton pressed ...');
            },
          ),
          title: Text(
            'Adicionar Membros',
            style: FlutterFlowTheme.of(context).headlineSmall.override(
                  font: GoogleFonts.outfit(
                    fontWeight: FontWeight.w500,
                    fontStyle:
                        FlutterFlowTheme.of(context).headlineSmall.fontStyle,
                  ),
                  color: Color(0xFF14181B),
                  fontSize: 24,
                  letterSpacing: 0.0,
                  fontWeight: FontWeight.w500,
                  fontStyle:
                      FlutterFlowTheme.of(context).headlineSmall.fontStyle,
                ),
          ),
          actions: [],
          centerTitle: false,
          elevation: 0,
        ),
        body: SingleChildScrollView(
          child: Column(
            mainAxisSize: MainAxisSize.max,
            crossAxisAlignment: CrossAxisAlignment.start,
            children: [
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(16, 8, 16, 12),
                child: Row(
                  mainAxisSize: MainAxisSize.max,
                  children: [
                    Expanded(
                      child: TextFormField(
                        controller: _model.textController,
                        focusNode: _model.textFieldFocusNode,
                        onChanged: (_) => EasyDebounce.debounce(
                          '_model.textController',
                          Duration(milliseconds: 2000),
                          () => safeSetState(() {}),
                        ),
                        autofocus: true,
                        obscureText: false,
                        decoration: InputDecoration(
                          labelText: 'Pesquisar Membros...',
                          labelStyle:
                              FlutterFlowTheme.of(context).labelMedium.override(
                                    font: GoogleFonts.plusJakartaSans(
                                      fontWeight: FontWeight.normal,
                                      fontStyle: FlutterFlowTheme.of(context)
                                          .labelMedium
                                          .fontStyle,
                                    ),
                                    color: Color(0xFF57636C),
                                    fontSize: 14,
                                    letterSpacing: 0.0,
                                    fontWeight: FontWeight.normal,
                                    fontStyle: FlutterFlowTheme.of(context)
                                        .labelMedium
                                        .fontStyle,
                                  ),
                          enabledBorder: OutlineInputBorder(
                            borderSide: BorderSide(
                              color: Colors.white,
                              width: 2,
                            ),
                            borderRadius: BorderRadius.circular(12),
                          ),
                          focusedBorder: OutlineInputBorder(
                            borderSide: BorderSide(
                              color: Color(0xFF4B39EF),
                              width: 2,
                            ),
                            borderRadius: BorderRadius.circular(12),
                          ),
                          errorBorder: OutlineInputBorder(
                            borderSide: BorderSide(
                              color: Color(0xFFFF5963),
                              width: 2,
                            ),
                            borderRadius: BorderRadius.circular(12),
                          ),
                          focusedErrorBorder: OutlineInputBorder(
                            borderSide: BorderSide(
                              color: Color(0xFFFF5963),
                              width: 2,
                            ),
                            borderRadius: BorderRadius.circular(12),
                          ),
                          filled: true,
                          fillColor: Colors.white,
                        ),
                        style: FlutterFlowTheme.of(context).bodyMedium.override(
                              font: GoogleFonts.plusJakartaSans(
                                fontWeight: FontWeight.normal,
                                fontStyle: FlutterFlowTheme.of(context)
                                    .bodyMedium
                                    .fontStyle,
                              ),
                              color: Color(0xFF14181B),
                              fontSize: 14,
                              letterSpacing: 0.0,
                              fontWeight: FontWeight.normal,
                              fontStyle: FlutterFlowTheme.of(context)
                                  .bodyMedium
                                  .fontStyle,
                            ),
                        validator:
                            _model.textControllerValidator.asValidator(context),
                      ),
                    ),
                    Padding(
                      padding: EdgeInsetsDirectional.fromSTEB(12, 0, 0, 0),
                      child: FlutterFlowIconButton(
                        borderColor: Colors.transparent,
                        borderRadius: 30,
                        borderWidth: 1,
                        buttonSize: 44,
                        icon: Icon(
                          Icons.search_rounded,
                          color: Color(0xFF14181B),
                          size: 24,
                        ),
                        onPressed: () {
                          print('IconButton pressed ...');
                        },
                      ),
                    ),
                  ],
                ),
              ),
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(24, 0, 0, 0),
                child: Text(
                  'Personas',
                  style: FlutterFlowTheme.of(context).labelMedium.override(
                        font: GoogleFonts.plusJakartaSans(
                          fontWeight: FontWeight.normal,
                          fontStyle: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontStyle,
                        ),
                        color: Color(0xFF57636C),
                        fontSize: 14,
                        letterSpacing: 0.0,
                        fontWeight: FontWeight.normal,
                        fontStyle:
                            FlutterFlowTheme.of(context).labelMedium.fontStyle,
                      ),
                ),
              ),
              Container(
                width: double.infinity,
                height: 170,
                decoration: BoxDecoration(
                  color: Color(0xFFF1F4F8),
                ),
                child: ListView(
                  padding: EdgeInsets.zero,
                  primary: false,
                  shrinkWrap: true,
                  scrollDirection: Axis.horizontal,
                  children: [
                    Padding(
                      padding: EdgeInsetsDirectional.fromSTEB(16, 12, 12, 12),
                      child: Container(
                        width: 160,
                        height: 100,
                        decoration: BoxDecoration(
                          color: Colors.white,
                          boxShadow: [
                            BoxShadow(
                              blurRadius: 4,
                              color: Color(0x34090F13),
                              offset: Offset(
                                0.0,
                                2,
                              ),
                            )
                          ],
                          borderRadius: BorderRadius.circular(8),
                        ),
                        child: Padding(
                          padding: EdgeInsets.all(12),
                          child: Column(
                            mainAxisSize: MainAxisSize.max,
                            mainAxisAlignment: MainAxisAlignment.center,
                            children: [
                              ClipRRect(
                                borderRadius: BorderRadius.circular(50),
                                child: Image.network(
                                  'https://images.unsplash.com/photo-1531427186611-ecfd6d936c79?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8cHJvZmlsZXxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=900&q=60',
                                  width: 60,
                                  height: 60,
                                  fit: BoxFit.cover,
                                ),
                              ),
                              Padding(
                                padding:
                                    EdgeInsetsDirectional.fromSTEB(0, 8, 0, 0),
                                child: Text(
                                  'Diego Costa',
                                  style: FlutterFlowTheme.of(context)
                                      .bodyMedium
                                      .override(
                                        font: GoogleFonts.plusJakartaSans(
                                          fontWeight: FontWeight.normal,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .bodyMedium
                                                  .fontStyle,
                                        ),
                                        color: Color(0xFF14181B),
                                        fontSize: 14,
                                        letterSpacing: 0.0,
                                        fontWeight: FontWeight.normal,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .bodyMedium
                                            .fontStyle,
                                      ),
                                ),
                              ),
                              Padding(
                                padding:
                                    EdgeInsetsDirectional.fromSTEB(0, 4, 0, 0),
                                child: Text(
                                  'Remover',
                                  style: FlutterFlowTheme.of(context)
                                      .labelSmall
                                      .override(
                                        font: GoogleFonts.plusJakartaSans(
                                          fontWeight: FontWeight.normal,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .labelSmall
                                                  .fontStyle,
                                        ),
                                        color: Color(0xFF57636C),
                                        fontSize: 12,
                                        letterSpacing: 0.0,
                                        fontWeight: FontWeight.normal,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .labelSmall
                                            .fontStyle,
                                      ),
                                ),
                              ),
                            ],
                          ),
                        ),
                      ),
                    ),
                    Padding(
                      padding: EdgeInsetsDirectional.fromSTEB(0, 12, 12, 12),
                      child: Container(
                        width: 160,
                        height: 100,
                        decoration: BoxDecoration(
                          color: Colors.white,
                          boxShadow: [
                            BoxShadow(
                              blurRadius: 4,
                              color: Color(0x34090F13),
                              offset: Offset(
                                0.0,
                                2,
                              ),
                            )
                          ],
                          borderRadius: BorderRadius.circular(8),
                        ),
                        child: Padding(
                          padding: EdgeInsets.all(12),
                          child: Column(
                            mainAxisSize: MainAxisSize.max,
                            mainAxisAlignment: MainAxisAlignment.center,
                            children: [
                              ClipRRect(
                                borderRadius: BorderRadius.circular(50),
                                child: Image.network(
                                  'https://images.unsplash.com/photo-1614436163996-25cee5f54290?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTJ8fHVzZXJ8ZW58MHx8MHx8&auto=format&fit=crop&w=900&q=60',
                                  width: 60,
                                  height: 60,
                                  fit: BoxFit.cover,
                                ),
                              ),
                              Padding(
                                padding:
                                    EdgeInsetsDirectional.fromSTEB(0, 8, 0, 0),
                                child: Text(
                                  'Mariana',
                                  style: FlutterFlowTheme.of(context)
                                      .bodyMedium
                                      .override(
                                        font: GoogleFonts.plusJakartaSans(
                                          fontWeight: FontWeight.normal,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .bodyMedium
                                                  .fontStyle,
                                        ),
                                        color: Color(0xFF14181B),
                                        fontSize: 14,
                                        letterSpacing: 0.0,
                                        fontWeight: FontWeight.normal,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .bodyMedium
                                            .fontStyle,
                                      ),
                                ),
                              ),
                              Padding(
                                padding:
                                    EdgeInsetsDirectional.fromSTEB(0, 4, 0, 0),
                                child: Text(
                                  'Remover',
                                  style: FlutterFlowTheme.of(context)
                                      .labelSmall
                                      .override(
                                        font: GoogleFonts.plusJakartaSans(
                                          fontWeight: FontWeight.normal,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .labelSmall
                                                  .fontStyle,
                                        ),
                                        color: Color(0xFF57636C),
                                        fontSize: 12,
                                        letterSpacing: 0.0,
                                        fontWeight: FontWeight.normal,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .labelSmall
                                            .fontStyle,
                                      ),
                                ),
                              ),
                            ],
                          ),
                        ),
                      ),
                    ),
                    Padding(
                      padding: EdgeInsetsDirectional.fromSTEB(0, 12, 12, 12),
                      child: Container(
                        width: 160,
                        height: 100,
                        decoration: BoxDecoration(
                          color: Colors.white,
                          boxShadow: [
                            BoxShadow(
                              blurRadius: 4,
                              color: Color(0x34090F13),
                              offset: Offset(
                                0.0,
                                2,
                              ),
                            )
                          ],
                          borderRadius: BorderRadius.circular(8),
                        ),
                        child: Padding(
                          padding: EdgeInsets.all(12),
                          child: Column(
                            mainAxisSize: MainAxisSize.max,
                            mainAxisAlignment: MainAxisAlignment.center,
                            children: [
                              ClipRRect(
                                borderRadius: BorderRadius.circular(50),
                                child: Image.network(
                                  'https://images.unsplash.com/photo-1521572267360-ee0c2909d518?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MjJ8fHByb2ZpbGV8ZW58MHx8MHx8&auto=format&fit=crop&w=900&q=60',
                                  width: 60,
                                  height: 60,
                                  fit: BoxFit.cover,
                                ),
                              ),
                              Align(
                                alignment: AlignmentDirectional(0, 0),
                                child: Padding(
                                  padding: EdgeInsetsDirectional.fromSTEB(
                                      0, 8, 0, 0),
                                  child: Text(
                                    'Lucas Ferreira',
                                    style: FlutterFlowTheme.of(context)
                                        .bodyMedium
                                        .override(
                                          font: GoogleFonts.plusJakartaSans(
                                            fontWeight: FontWeight.normal,
                                            fontStyle:
                                                FlutterFlowTheme.of(context)
                                                    .bodyMedium
                                                    .fontStyle,
                                          ),
                                          color: Color(0xFF14181B),
                                          fontSize: 14,
                                          letterSpacing: 0.0,
                                          fontWeight: FontWeight.normal,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .bodyMedium
                                                  .fontStyle,
                                        ),
                                  ),
                                ),
                              ),
                              Padding(
                                padding:
                                    EdgeInsetsDirectional.fromSTEB(0, 4, 0, 0),
                                child: Text(
                                  'Remover',
                                  style: FlutterFlowTheme.of(context)
                                      .labelSmall
                                      .override(
                                        font: GoogleFonts.plusJakartaSans(
                                          fontWeight: FontWeight.normal,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .labelSmall
                                                  .fontStyle,
                                        ),
                                        color: Color(0xFF57636C),
                                        fontSize: 12,
                                        letterSpacing: 0.0,
                                        fontWeight: FontWeight.normal,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .labelSmall
                                            .fontStyle,
                                      ),
                                ),
                              ),
                            ],
                          ),
                        ),
                      ),
                    ),
                  ],
                ),
              ),
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(24, 0, 0, 0),
                child: Text(
                  'Adicionar Membros ',
                  style: FlutterFlowTheme.of(context).labelMedium.override(
                        font: GoogleFonts.plusJakartaSans(
                          fontWeight: FontWeight.normal,
                          fontStyle: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontStyle,
                        ),
                        color: Color(0xFF57636C),
                        fontSize: 14,
                        letterSpacing: 0.0,
                        fontWeight: FontWeight.normal,
                        fontStyle:
                            FlutterFlowTheme.of(context).labelMedium.fontStyle,
                      ),
                ),
              ),
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(0, 12, 0, 44),
                child: ListView(
                  padding: EdgeInsets.zero,
                  primary: false,
                  shrinkWrap: true,
                  scrollDirection: Axis.vertical,
                  children: [
                    Padding(
                      padding: EdgeInsetsDirectional.fromSTEB(16, 4, 16, 8),
                      child: Container(
                        width: double.infinity,
                        height: 60,
                        decoration: BoxDecoration(
                          color: Colors.white,
                          boxShadow: [
                            BoxShadow(
                              blurRadius: 4,
                              color: Color(0x32000000),
                              offset: Offset(
                                0.0,
                                2,
                              ),
                            )
                          ],
                          borderRadius: BorderRadius.circular(8),
                        ),
                        child: Padding(
                          padding: EdgeInsetsDirectional.fromSTEB(8, 0, 8, 0),
                          child: Row(
                            mainAxisSize: MainAxisSize.max,
                            mainAxisAlignment: MainAxisAlignment.spaceBetween,
                            children: [
                              ClipRRect(
                                borderRadius: BorderRadius.circular(26),
                                child: Image.network(
                                  'https://images.unsplash.com/photo-1614436163996-25cee5f54290?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTJ8fHVzZXJ8ZW58MHx8MHx8&auto=format&fit=crop&w=900&q=60',
                                  width: 36,
                                  height: 36,
                                  fit: BoxFit.cover,
                                ),
                              ),
                              Expanded(
                                child: Padding(
                                  padding: EdgeInsetsDirectional.fromSTEB(
                                      12, 0, 0, 0),
                                  child: Column(
                                    mainAxisSize: MainAxisSize.max,
                                    mainAxisAlignment: MainAxisAlignment.center,
                                    crossAxisAlignment:
                                        CrossAxisAlignment.start,
                                    children: [
                                      Text(
                                        'Mariana',
                                        style: FlutterFlowTheme.of(context)
                                            .bodyMedium
                                            .override(
                                              font: GoogleFonts.plusJakartaSans(
                                                fontWeight: FontWeight.normal,
                                                fontStyle:
                                                    FlutterFlowTheme.of(context)
                                                        .bodyMedium
                                                        .fontStyle,
                                              ),
                                              color: Color(0xFF14181B),
                                              fontSize: 14,
                                              letterSpacing: 0.0,
                                              fontWeight: FontWeight.normal,
                                              fontStyle:
                                                  FlutterFlowTheme.of(context)
                                                      .bodyMedium
                                                      .fontStyle,
                                            ),
                                      ),
                                      Row(
                                        mainAxisSize: MainAxisSize.max,
                                        children: [
                                          Padding(
                                            padding:
                                                EdgeInsetsDirectional.fromSTEB(
                                                    0, 4, 0, 0),
                                            child: Text(
                                              'mariana@domainname.com',
                                              style:
                                                  FlutterFlowTheme.of(context)
                                                      .labelMedium
                                                      .override(
                                                        font: GoogleFonts
                                                            .plusJakartaSans(
                                                          fontWeight:
                                                              FontWeight.normal,
                                                          fontStyle:
                                                              FlutterFlowTheme.of(
                                                                      context)
                                                                  .labelMedium
                                                                  .fontStyle,
                                                        ),
                                                        color:
                                                            Color(0xFF57636C),
                                                        fontSize: 14,
                                                        letterSpacing: 0.0,
                                                        fontWeight:
                                                            FontWeight.normal,
                                                        fontStyle:
                                                            FlutterFlowTheme.of(
                                                                    context)
                                                                .labelMedium
                                                                .fontStyle,
                                                      ),
                                            ),
                                          ),
                                        ],
                                      ),
                                    ],
                                  ),
                                ),
                              ),
                              FFButtonWidget(
                                onPressed: () {
                                  print('Button pressed ...');
                                },
                                text: 'View',
                                options: FFButtonOptions(
                                  width: 70,
                                  height: 36,
                                  padding: EdgeInsetsDirectional.fromSTEB(
                                      0, 0, 0, 0),
                                  iconPadding: EdgeInsetsDirectional.fromSTEB(
                                      0, 0, 0, 0),
                                  color: Color(0xFF44BB33),
                                  textStyle: FlutterFlowTheme.of(context)
                                      .bodyMedium
                                      .override(
                                        font: GoogleFonts.outfit(
                                          fontWeight: FontWeight.normal,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .bodyMedium
                                                  .fontStyle,
                                        ),
                                        color: Colors.white,
                                        fontSize: 14,
                                        letterSpacing: 0.0,
                                        fontWeight: FontWeight.normal,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .bodyMedium
                                            .fontStyle,
                                      ),
                                  elevation: 2,
                                  borderSide: BorderSide(
                                    color: Colors.transparent,
                                    width: 1,
                                  ),
                                  borderRadius: BorderRadius.circular(8),
                                ),
                              ),
                            ],
                          ),
                        ),
                      ),
                    ),
                    Padding(
                      padding: EdgeInsetsDirectional.fromSTEB(16, 4, 16, 8),
                      child: Container(
                        width: double.infinity,
                        height: 60,
                        decoration: BoxDecoration(
                          color: Colors.white,
                          boxShadow: [
                            BoxShadow(
                              blurRadius: 4,
                              color: Color(0x32000000),
                              offset: Offset(
                                0.0,
                                2,
                              ),
                            )
                          ],
                          borderRadius: BorderRadius.circular(8),
                        ),
                        child: Padding(
                          padding: EdgeInsetsDirectional.fromSTEB(8, 0, 8, 0),
                          child: Row(
                            mainAxisSize: MainAxisSize.max,
                            mainAxisAlignment: MainAxisAlignment.spaceBetween,
                            children: [
                              ClipRRect(
                                borderRadius: BorderRadius.circular(26),
                                child: Image.network(
                                  'https://images.unsplash.com/photo-1531427186611-ecfd6d936c79?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8cHJvZmlsZXxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=900&q=60',
                                  width: 36,
                                  height: 36,
                                  fit: BoxFit.cover,
                                ),
                              ),
                              Expanded(
                                child: Padding(
                                  padding: EdgeInsetsDirectional.fromSTEB(
                                      12, 0, 0, 0),
                                  child: Column(
                                    mainAxisSize: MainAxisSize.max,
                                    mainAxisAlignment: MainAxisAlignment.center,
                                    crossAxisAlignment:
                                        CrossAxisAlignment.start,
                                    children: [
                                      Text(
                                        'Diego Costa',
                                        style: FlutterFlowTheme.of(context)
                                            .bodyMedium
                                            .override(
                                              font: GoogleFonts.plusJakartaSans(
                                                fontWeight: FontWeight.normal,
                                                fontStyle:
                                                    FlutterFlowTheme.of(context)
                                                        .bodyMedium
                                                        .fontStyle,
                                              ),
                                              color: Color(0xFF14181B),
                                              fontSize: 14,
                                              letterSpacing: 0.0,
                                              fontWeight: FontWeight.normal,
                                              fontStyle:
                                                  FlutterFlowTheme.of(context)
                                                      .bodyMedium
                                                      .fontStyle,
                                            ),
                                      ),
                                      Row(
                                        mainAxisSize: MainAxisSize.max,
                                        children: [
                                          Padding(
                                            padding:
                                                EdgeInsetsDirectional.fromSTEB(
                                                    0, 4, 0, 0),
                                            child: Text(
                                              'diego@domainname.com',
                                              style:
                                                  FlutterFlowTheme.of(context)
                                                      .labelMedium
                                                      .override(
                                                        font: GoogleFonts
                                                            .plusJakartaSans(
                                                          fontWeight:
                                                              FontWeight.normal,
                                                          fontStyle:
                                                              FlutterFlowTheme.of(
                                                                      context)
                                                                  .labelMedium
                                                                  .fontStyle,
                                                        ),
                                                        color:
                                                            Color(0xFF57636C),
                                                        fontSize: 14,
                                                        letterSpacing: 0.0,
                                                        fontWeight:
                                                            FontWeight.normal,
                                                        fontStyle:
                                                            FlutterFlowTheme.of(
                                                                    context)
                                                                .labelMedium
                                                                .fontStyle,
                                                      ),
                                            ),
                                          ),
                                        ],
                                      ),
                                    ],
                                  ),
                                ),
                              ),
                              FFButtonWidget(
                                onPressed: () {
                                  print('Button pressed ...');
                                },
                                text: 'View',
                                options: FFButtonOptions(
                                  width: 70,
                                  height: 36,
                                  padding: EdgeInsetsDirectional.fromSTEB(
                                      0, 0, 0, 0),
                                  iconPadding: EdgeInsetsDirectional.fromSTEB(
                                      0, 0, 0, 0),
                                  color: Color(0xFF44BB33),
                                  textStyle: FlutterFlowTheme.of(context)
                                      .bodyMedium
                                      .override(
                                        font: GoogleFonts.outfit(
                                          fontWeight: FontWeight.normal,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .bodyMedium
                                                  .fontStyle,
                                        ),
                                        color: Colors.white,
                                        fontSize: 14,
                                        letterSpacing: 0.0,
                                        fontWeight: FontWeight.normal,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .bodyMedium
                                            .fontStyle,
                                      ),
                                  elevation: 2,
                                  borderSide: BorderSide(
                                    color: Colors.transparent,
                                    width: 1,
                                  ),
                                  borderRadius: BorderRadius.circular(8),
                                ),
                              ),
                            ],
                          ),
                        ),
                      ),
                    ),
                    Padding(
                      padding: EdgeInsetsDirectional.fromSTEB(16, 4, 16, 8),
                      child: Container(
                        width: double.infinity,
                        height: 60,
                        decoration: BoxDecoration(
                          color: Colors.white,
                          boxShadow: [
                            BoxShadow(
                              blurRadius: 4,
                              color: Color(0x32000000),
                              offset: Offset(
                                0.0,
                                2,
                              ),
                            )
                          ],
                          borderRadius: BorderRadius.circular(8),
                        ),
                        child: Padding(
                          padding: EdgeInsetsDirectional.fromSTEB(8, 0, 8, 0),
                          child: Row(
                            mainAxisSize: MainAxisSize.max,
                            mainAxisAlignment: MainAxisAlignment.spaceBetween,
                            children: [
                              ClipRRect(
                                borderRadius: BorderRadius.circular(26),
                                child: Image.network(
                                  'https://images.unsplash.com/photo-1521572267360-ee0c2909d518?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MjJ8fHByb2ZpbGV8ZW58MHx8MHx8&auto=format&fit=crop&w=900&q=60',
                                  width: 36,
                                  height: 36,
                                  fit: BoxFit.cover,
                                ),
                              ),
                              Expanded(
                                child: Padding(
                                  padding: EdgeInsetsDirectional.fromSTEB(
                                      12, 0, 0, 0),
                                  child: Column(
                                    mainAxisSize: MainAxisSize.max,
                                    mainAxisAlignment: MainAxisAlignment.center,
                                    crossAxisAlignment:
                                        CrossAxisAlignment.start,
                                    children: [
                                      Text(
                                        'Lucas Ferreira',
                                        style: FlutterFlowTheme.of(context)
                                            .bodyMedium
                                            .override(
                                              font: GoogleFonts.plusJakartaSans(
                                                fontWeight: FontWeight.normal,
                                                fontStyle:
                                                    FlutterFlowTheme.of(context)
                                                        .bodyMedium
                                                        .fontStyle,
                                              ),
                                              color: Color(0xFF14181B),
                                              fontSize: 14,
                                              letterSpacing: 0.0,
                                              fontWeight: FontWeight.normal,
                                              fontStyle:
                                                  FlutterFlowTheme.of(context)
                                                      .bodyMedium
                                                      .fontStyle,
                                            ),
                                      ),
                                      Row(
                                        mainAxisSize: MainAxisSize.max,
                                        children: [
                                          Padding(
                                            padding:
                                                EdgeInsetsDirectional.fromSTEB(
                                                    0, 4, 0, 0),
                                            child: Text(
                                              'lucas@domainname.com',
                                              style:
                                                  FlutterFlowTheme.of(context)
                                                      .labelMedium
                                                      .override(
                                                        font: GoogleFonts
                                                            .plusJakartaSans(
                                                          fontWeight:
                                                              FontWeight.normal,
                                                          fontStyle:
                                                              FlutterFlowTheme.of(
                                                                      context)
                                                                  .labelMedium
                                                                  .fontStyle,
                                                        ),
                                                        color:
                                                            Color(0xFF57636C),
                                                        fontSize: 14,
                                                        letterSpacing: 0.0,
                                                        fontWeight:
                                                            FontWeight.normal,
                                                        fontStyle:
                                                            FlutterFlowTheme.of(
                                                                    context)
                                                                .labelMedium
                                                                .fontStyle,
                                                      ),
                                            ),
                                          ),
                                        ],
                                      ),
                                    ],
                                  ),
                                ),
                              ),
                              FFButtonWidget(
                                onPressed: () {
                                  print('Button pressed ...');
                                },
                                text: 'View',
                                options: FFButtonOptions(
                                  width: 70,
                                  height: 36,
                                  padding: EdgeInsetsDirectional.fromSTEB(
                                      0, 0, 0, 0),
                                  iconPadding: EdgeInsetsDirectional.fromSTEB(
                                      0, 0, 0, 0),
                                  color: Color(0xFF44BB33),
                                  textStyle: FlutterFlowTheme.of(context)
                                      .bodyMedium
                                      .override(
                                        font: GoogleFonts.outfit(
                                          fontWeight: FontWeight.normal,
                                          fontStyle:
                                              FlutterFlowTheme.of(context)
                                                  .bodyMedium
                                                  .fontStyle,
                                        ),
                                        color: Colors.white,
                                        fontSize: 14,
                                        letterSpacing: 0.0,
                                        fontWeight: FontWeight.normal,
                                        fontStyle: FlutterFlowTheme.of(context)
                                            .bodyMedium
                                            .fontStyle,
                                      ),
                                  elevation: 2,
                                  borderSide: BorderSide(
                                    color: Colors.transparent,
                                    width: 1,
                                  ),
                                  borderRadius: BorderRadius.circular(8),
                                ),
                              ),
                            ],
                          ),
                        ),
                      ),
                    ),
                  ],
                ),
              ),
            ],
          ),
        ),
      ),
    );
  }
}



import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import '/index.dart';
import 'package:badges/badges.dart' as badges;
import 'package:flutter/material.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:provider/provider.dart';

import 'cart_badge_model.dart';
export 'cart_badge_model.dart';

class CartBadgeWidget extends StatefulWidget {
  const CartBadgeWidget({super.key});

  @override
  State<CartBadgeWidget> createState() => _CartBadgeWidgetState();
}

class _CartBadgeWidgetState extends State<CartBadgeWidget> {
  late CartBadgeModel _model;

  @override
  void setState(VoidCallback callback) {
    super.setState(callback);
    _model.onUpdate();
  }

  @override
  void initState() {
    super.initState();
    _model = createModel(context, () => CartBadgeModel());
  }

  @override
  void dispose() {
    _model.maybeDispose();

    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    context.watch<FFAppState>();

    return Padding(
      padding: EdgeInsetsDirectional.fromSTEB(0, 8, 16, 0),
      child: InkWell(
        splashColor: Colors.transparent,
        focusColor: Colors.transparent,
        hoverColor: Colors.transparent,
        highlightColor: Colors.transparent,
        onTap: () async {
          context.pushNamed(
            DetalhesReservasWidget.routeName,
            extra: <String, dynamic>{
              kTransitionInfoKey: TransitionInfo(
                hasTransition: true,
                transitionType: PageTransitionType.bottomToTop,
                duration: Duration(milliseconds: 300),
              ),
            },
          );
        },
        child: badges.Badge(
          badgeContent: Text(
            valueOrDefault<String>(
              FFAppState().myCart.length.toString(),
              '0',
            ),
            style: FlutterFlowTheme.of(context).titleSmall.override(
                  font: GoogleFonts.interTight(
                    fontWeight:
                        FlutterFlowTheme.of(context).titleSmall.fontWeight,
                    fontStyle:
                        FlutterFlowTheme.of(context).titleSmall.fontStyle,
                  ),
                  color: FFAppState().myCart.length >= 1
                      ? FlutterFlowTheme.of(context).info
                      : FlutterFlowTheme.of(context).primaryText,
                  letterSpacing: 0.0,
                  fontWeight:
                      FlutterFlowTheme.of(context).titleSmall.fontWeight,
                  fontStyle: FlutterFlowTheme.of(context).titleSmall.fontStyle,
                ),
          ),
          showBadge: true,
          shape: badges.BadgeShape.circle,
          badgeColor: FFAppState().myCart.length >= 1
              ? FlutterFlowTheme.of(context).primary
              : FlutterFlowTheme.of(context).primaryBackground,
          elevation: 4,
          padding: EdgeInsets.all(8),
          position: badges.BadgePosition.topEnd(),
          animationType: badges.BadgeAnimationType.scale,
          toAnimate: true,
          child: Padding(
            padding: EdgeInsetsDirectional.fromSTEB(16, 0, 0, 0),
            child: Icon(
              Icons.shopping_cart_outlined,
              color: FlutterFlowTheme.of(context).secondaryText,
              size: 32,
            ),
          ),
        ),
      ),
    );
  }
}


import '/flutter_flow/flutter_flow_icon_button.dart';
import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import '/reservation_flow/cart_reservation/cart_reservation_widget.dart';
import 'dart:ui';
import '/flutter_flow/custom_functions.dart' as functions;
import 'package:auto_size_text/auto_size_text.dart';
import 'package:flutter/gestures.dart';
import 'package:flutter/material.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:provider/provider.dart';

import 'cart_summary_model.dart';
export 'cart_summary_model.dart';

class CartSummaryWidget extends StatefulWidget {
  const CartSummaryWidget({
    super.key,
    bool? showTotal,
  }) : this.showTotal = showTotal ?? false;

  final bool showTotal;

  @override
  State<CartSummaryWidget> createState() => _CartSummaryWidgetState();
}

class _CartSummaryWidgetState extends State<CartSummaryWidget> {
  late CartSummaryModel _model;

  @override
  void setState(VoidCallback callback) {
    super.setState(callback);
    _model.onUpdate();
  }

  @override
  void initState() {
    super.initState();
    _model = createModel(context, () => CartSummaryModel());
  }

  @override
  void dispose() {
    _model.maybeDispose();

    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    context.watch<FFAppState>();

    return Container(
      constraints: BoxConstraints(
        maxWidth: 750,
      ),
      decoration: BoxDecoration(
        color: FlutterFlowTheme.of(context).secondaryBackground,
        boxShadow: [
          BoxShadow(
            blurRadius: 4,
            color: Color(0x33000000),
            offset: Offset(
              0,
              2,
            ),
          )
        ],
        borderRadius: BorderRadius.circular(12),
      ),
      child: Padding(
        padding: EdgeInsets.all(16),
        child: Column(
          mainAxisSize: MainAxisSize.max,
          crossAxisAlignment: CrossAxisAlignment.start,
          children: [
            Text(
              'Sua Seleção',
              style: FlutterFlowTheme.of(context).headlineSmall.override(
                    font: GoogleFonts.interTight(
                      fontWeight:
                          FlutterFlowTheme.of(context).headlineSmall.fontWeight,
                      fontStyle:
                          FlutterFlowTheme.of(context).headlineSmall.fontStyle,
                    ),
                    letterSpacing: 0.0,
                    fontWeight:
                        FlutterFlowTheme.of(context).headlineSmall.fontWeight,
                    fontStyle:
                        FlutterFlowTheme.of(context).headlineSmall.fontStyle,
                  ),
            ),
            Padding(
              padding: EdgeInsetsDirectional.fromSTEB(0, 4, 0, 12),
              child: Text(
                'Abaixo está a listagem dos quartos selecionados',
                style: FlutterFlowTheme.of(context).labelMedium.override(
                      font: GoogleFonts.inter(
                        fontWeight:
                            FlutterFlowTheme.of(context).labelMedium.fontWeight,
                        fontStyle:
                            FlutterFlowTheme.of(context).labelMedium.fontStyle,
                      ),
                      letterSpacing: 0.0,
                      fontWeight:
                          FlutterFlowTheme.of(context).labelMedium.fontWeight,
                      fontStyle:
                          FlutterFlowTheme.of(context).labelMedium.fontStyle,
                    ),
              ),
            ),
            Builder(
              builder: (context) {
                final cartItems =
                    FFAppState().myReservation.map((e) => e.id).toList();

                return ListView.builder(
                  padding: EdgeInsets.zero,
                  shrinkWrap: true,
                  scrollDirection: Axis.vertical,
                  itemCount: cartItems.length,
                  itemBuilder: (context, cartItemsIndex) {
                    final cartItemsItem = cartItems[cartItemsIndex];
                    return wrapWithModel(
                      model: _model.cartReservationModels.getModel(
                        cartItemsItem.id,
                        cartItemsIndex,
                      ),
                      updateCallback: () => safeSetState(() {}),
                      updateOnChange: true,
                      child: CartReservationWidget(
                        key: Key(
                          'Keykid_${cartItemsItem.id}',
                        ),
                        product: cartItemsItem,
                        cartItem: true,
                      ),
                    );
                  },
                );
              },
            ),
            if (widget!.showTotal)
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(0, 8, 0, 8),
                child: Row(
                  mainAxisSize: MainAxisSize.max,
                  mainAxisAlignment: MainAxisAlignment.spaceBetween,
                  children: [
                    Row(
                      mainAxisSize: MainAxisSize.max,
                      children: [
                        Text(
                          'Sub Total',
                          style: FlutterFlowTheme.of(context)
                              .titleMedium
                              .override(
                                font: GoogleFonts.outfit(
                                  fontWeight: FontWeight.w500,
                                  fontStyle: FlutterFlowTheme.of(context)
                                      .titleMedium
                                      .fontStyle,
                                ),
                                color:
                                    FlutterFlowTheme.of(context).secondaryText,
                                fontSize: 20,
                                letterSpacing: 0.0,
                                fontWeight: FontWeight.w500,
                                fontStyle: FlutterFlowTheme.of(context)
                                    .titleMedium
                                    .fontStyle,
                              ),
                        ),
                        FlutterFlowIconButton(
                          borderColor: Colors.transparent,
                          borderRadius: 30,
                          borderWidth: 1,
                          buttonSize: 36,
                          icon: Icon(
                            Icons.info_outlined,
                            color: FlutterFlowTheme.of(context).secondaryText,
                            size: 18,
                          ),
                          onPressed: () {
                            print('IconButton pressed ...');
                          },
                        ),
                      ],
                    ),
                    Text(
                      valueOrDefault<String>(
                        formatNumber(
                          functions.priceSummary(
                              FFAppState().myCartSummary.toList()),
                          formatType: FormatType.decimal,
                          decimalType: DecimalType.automatic,
                          currency: '\$',
                        ),
                        '0',
                      ),
                      style: FlutterFlowTheme.of(context).displaySmall.override(
                            font: GoogleFonts.interTight(
                              fontWeight: FlutterFlowTheme.of(context)
                                  .displaySmall
                                  .fontWeight,
                              fontStyle: FlutterFlowTheme.of(context)
                                  .displaySmall
                                  .fontStyle,
                            ),
                            letterSpacing: 0.0,
                            fontWeight: FlutterFlowTheme.of(context)
                                .displaySmall
                                .fontWeight,
                            fontStyle: FlutterFlowTheme.of(context)
                                .displaySmall
                                .fontStyle,
                          ),
                    ),
                  ],
                ),
              ),
          ],
        ),
      ),
    );
  }
}


import '/flutter_flow/flutter_flow_animations.dart';
import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import '/flutter_flow/flutter_flow_widgets.dart';
import 'dart:math';
import 'dart:ui';
import 'package:flutter/gestures.dart';
import 'package:flutter/material.dart';
import 'package:flutter/scheduler.dart';
import 'package:flutter_animate/flutter_animate.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:provider/provider.dart';

import 'descricao_quartos_model.dart';
export 'descricao_quartos_model.dart';

class DescricaoQuartosWidget extends StatefulWidget {
  const DescricaoQuartosWidget({super.key});

  @override
  State<DescricaoQuartosWidget> createState() => _DescricaoQuartosWidgetState();
}

class _DescricaoQuartosWidgetState extends State<DescricaoQuartosWidget>
    with TickerProviderStateMixin {
  late DescricaoQuartosModel _model;

  final animationsMap = <String, AnimationInfo>{};

  @override
  void setState(VoidCallback callback) {
    super.setState(callback);
    _model.onUpdate();
  }

  @override
  void initState() {
    super.initState();
    _model = createModel(context, () => DescricaoQuartosModel());

    animationsMap.addAll({
      'columnOnPageLoadAnimation': AnimationInfo(
        trigger: AnimationTrigger.onPageLoad,
        effectsBuilder: () => [
          VisibilityEffect(duration: 200.ms),
          FadeEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 500.0.ms,
            begin: 0.0,
            end: 1.0,
          ),
          TiltEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 500.0.ms,
            begin: Offset(-1.396, 0),
            end: Offset(0, 0),
          ),
          ScaleEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 500.0.ms,
            begin: Offset(0.7, 0.7),
            end: Offset(1.0, 1.0),
          ),
          MoveEffect(
            curve: Curves.easeInOut,
            delay: 200.0.ms,
            duration: 500.0.ms,
            begin: Offset(0.0, 30.0),
            end: Offset(0.0, 0.0),
          ),
        ],
      ),
    });
  }

  @override
  void dispose() {
    _model.maybeDispose();

    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return Padding(
      padding: EdgeInsets.all(16),
      child: Column(
        mainAxisSize: MainAxisSize.max,
        crossAxisAlignment: CrossAxisAlignment.start,
        children: [
          Text(
            'Suite casal premium',
            style: FlutterFlowTheme.of(context).headlineMedium.override(
                  font: GoogleFonts.outfit(
                    fontWeight: FontWeight.w500,
                    fontStyle:
                        FlutterFlowTheme.of(context).headlineMedium.fontStyle,
                  ),
                  color: Color(0xFF15161E),
                  fontSize: 24,
                  letterSpacing: 0.0,
                  fontWeight: FontWeight.w500,
                  fontStyle:
                      FlutterFlowTheme.of(context).headlineMedium.fontStyle,
                ),
          ),
          Row(
            mainAxisSize: MainAxisSize.max,
            mainAxisAlignment: MainAxisAlignment.spaceBetween,
            children: [
              RichText(
                textScaler: MediaQuery.of(context).textScaler,
                text: TextSpan(
                  children: [
                    TextSpan(
                      text: 'SOHO',
                      style: TextStyle(),
                    ),
                    TextSpan(
                      text: ' || ',
                      style: TextStyle(),
                    ),
                    TextSpan(
                      text: '0.4 mi',
                      style: TextStyle(),
                    )
                  ],
                  style: FlutterFlowTheme.of(context).labelMedium.override(
                        font: GoogleFonts.outfit(
                          fontWeight: FontWeight.w500,
                          fontStyle: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontStyle,
                        ),
                        color: Color(0xFF606A85),
                        fontSize: 14,
                        letterSpacing: 0.0,
                        fontWeight: FontWeight.w500,
                        fontStyle:
                            FlutterFlowTheme.of(context).labelMedium.fontStyle,
                      ),
                ),
              ),
              Container(
                height: 32,
                decoration: BoxDecoration(
                  color: Color(0x4C39D2C0),
                  borderRadius: BorderRadius.circular(12),
                  border: Border.all(
                    color: Color(0xFF39D2C0),
                    width: 2,
                  ),
                ),
                child: Align(
                  alignment: AlignmentDirectional(0, 0),
                  child: Padding(
                    padding: EdgeInsetsDirectional.fromSTEB(12, 0, 12, 0),
                    child: Text(
                      'Disponivel - Faça uma reserva',
                      style: FlutterFlowTheme.of(context).bodyMedium.override(
                            font: GoogleFonts.figtree(
                              fontWeight: FontWeight.w600,
                              fontStyle: FlutterFlowTheme.of(context)
                                  .bodyMedium
                                  .fontStyle,
                            ),
                            color: Color(0xFF15161E),
                            fontSize: 14,
                            letterSpacing: 0.0,
                            fontWeight: FontWeight.w600,
                            fontStyle: FlutterFlowTheme.of(context)
                                .bodyMedium
                                .fontStyle,
                          ),
                    ),
                  ),
                ),
              ),
            ].divide(SizedBox(width: 8)),
          ),
          Divider(
            height: 16,
            thickness: 1,
            color: Color(0xFFE5E7EB),
          ),
          Text(
            'Valor',
            style: FlutterFlowTheme.of(context).labelMedium.override(
                  font: GoogleFonts.outfit(
                    fontWeight: FontWeight.w500,
                    fontStyle:
                        FlutterFlowTheme.of(context).labelMedium.fontStyle,
                  ),
                  color: Color(0xFF606A85),
                  fontSize: 14,
                  letterSpacing: 0.0,
                  fontWeight: FontWeight.w500,
                  fontStyle: FlutterFlowTheme.of(context).labelMedium.fontStyle,
                ),
          ),
          Row(
            mainAxisSize: MainAxisSize.max,
            mainAxisAlignment: MainAxisAlignment.spaceBetween,
            children: [
              Row(
                mainAxisSize: MainAxisSize.max,
                children: [
                  Text(
                    'R\$450,00',
                    style: FlutterFlowTheme.of(context).bodyLarge.override(
                          font: GoogleFonts.figtree(
                            fontWeight: FontWeight.w600,
                            fontStyle: FlutterFlowTheme.of(context)
                                .bodyLarge
                                .fontStyle,
                          ),
                          color: Color(0xFF15161E),
                          fontSize: 16,
                          letterSpacing: 0.0,
                          fontWeight: FontWeight.w600,
                          fontStyle:
                              FlutterFlowTheme.of(context).bodyLarge.fontStyle,
                        ),
                  ),
                  Text(
                    'por dia',
                    style: FlutterFlowTheme.of(context).labelMedium.override(
                          font: GoogleFonts.outfit(
                            fontWeight: FontWeight.w500,
                            fontStyle: FlutterFlowTheme.of(context)
                                .labelMedium
                                .fontStyle,
                          ),
                          color: Color(0xFF606A85),
                          fontSize: 14,
                          letterSpacing: 0.0,
                          fontWeight: FontWeight.w500,
                          fontStyle: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontStyle,
                        ),
                  ),
                ].divide(SizedBox(width: 4)),
              ),
              FFButtonWidget(
                onPressed: () async {
                  FFAppState().addToMyReservation();
                  safeSetState(() {});
                },
                text: 'Reserve',
                options: FFButtonOptions(
                  height: 40,
                  padding: EdgeInsetsDirectional.fromSTEB(16, 0, 16, 0),
                  iconPadding: EdgeInsetsDirectional.fromSTEB(0, 0, 0, 0),
                  color: FlutterFlowTheme.of(context).secondary,
                  textStyle: FlutterFlowTheme.of(context).titleSmall.override(
                        font: GoogleFonts.interTight(
                          fontWeight: FlutterFlowTheme.of(context)
                              .titleSmall
                              .fontWeight,
                          fontStyle:
                              FlutterFlowTheme.of(context).titleSmall.fontStyle,
                        ),
                        color: Colors.white,
                        letterSpacing: 0.0,
                        fontWeight:
                            FlutterFlowTheme.of(context).titleSmall.fontWeight,
                        fontStyle:
                            FlutterFlowTheme.of(context).titleSmall.fontStyle,
                      ),
                  elevation: 0,
                  borderRadius: BorderRadius.circular(8),
                ),
              ),
            ],
          ),
          Divider(
            height: 16,
            thickness: 1,
            color: Color(0xFFE5E7EB),
          ),
          Text(
            'Amenidades',
            style: FlutterFlowTheme.of(context).labelMedium.override(
                  font: GoogleFonts.outfit(
                    fontWeight: FontWeight.w500,
                    fontStyle:
                        FlutterFlowTheme.of(context).labelMedium.fontStyle,
                  ),
                  color: Color(0xFF606A85),
                  fontSize: 14,
                  letterSpacing: 0.0,
                  fontWeight: FontWeight.w500,
                  fontStyle: FlutterFlowTheme.of(context).labelMedium.fontStyle,
                ),
          ),
          Padding(
            padding: EdgeInsetsDirectional.fromSTEB(0, 0, 0, 1),
            child: Container(
              width: double.infinity,
              height: 60,
              decoration: BoxDecoration(
                color: Colors.white,
              ),
              child: Padding(
                padding: EdgeInsetsDirectional.fromSTEB(0, 4, 0, 4),
                child: Row(
                  mainAxisSize: MainAxisSize.max,
                  children: <Widget>[].divide(SizedBox(width: 12)),
                ),
              ),
            ),
          ),
          Divider(
            height: 16,
            thickness: 1,
            color: Color(0xFFE5E7EB),
          ),
          Text(
            'Description',
            style: FlutterFlowTheme.of(context).labelMedium.override(
                  font: GoogleFonts.outfit(
                    fontWeight: FontWeight.w500,
                    fontStyle:
                        FlutterFlowTheme.of(context).labelMedium.fontStyle,
                  ),
                  color: Color(0xFF606A85),
                  fontSize: 14,
                  letterSpacing: 0.0,
                  fontWeight: FontWeight.w500,
                  fontStyle: FlutterFlowTheme.of(context).labelMedium.fontStyle,
                ),
          ),
          Text(
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. ',
            style: FlutterFlowTheme.of(context).bodyMedium.override(
                  font: GoogleFonts.figtree(
                    fontWeight: FontWeight.w600,
                    fontStyle:
                        FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                  ),
                  color: Color(0xFF15161E),
                  fontSize: 14,
                  letterSpacing: 0.0,
                  fontWeight: FontWeight.w600,
                  fontStyle: FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                ),
          ),
          Divider(
            height: 16,
            thickness: 1,
            color: Color(0xFFE5E7EB),
          ),
        ].divide(SizedBox(height: 4)),
      ).animateOnPageLoad(animationsMap['columnOnPageLoadAnimation']!),
    );
  }
}


import '/auth/firebase_auth/auth_util.dart';
import '/backend/backend.dart';
import '/backend/firebase_storage/storage.dart';
import '/flutter_flow/flutter_flow_drop_down.dart';
import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import '/flutter_flow/flutter_flow_widgets.dart';
import '/flutter_flow/form_field_controller.dart';
import '/flutter_flow/upload_data.dart';
import 'dart:ui';
import 'package:cached_network_image/cached_network_image.dart';
import 'package:cloud_firestore/cloud_firestore.dart';
import 'package:flutter/material.dart';
import 'package:flutter/services.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:provider/provider.dart';

import 'edit_profile_auth2_model.dart';
export 'edit_profile_auth2_model.dart';

class EditProfileAuth2Widget extends StatefulWidget {
  const EditProfileAuth2Widget({
    super.key,
    String? title,
    String? confirmButtonText,
    required this.navigateAction,
  })  : this.title = title ?? 'Edit Profile',
        this.confirmButtonText = confirmButtonText ?? 'Save Changes';

  final String title;
  final String confirmButtonText;
  final Future Function()? navigateAction;

  @override
  State<EditProfileAuth2Widget> createState() => _EditProfileAuth2WidgetState();
}

class _EditProfileAuth2WidgetState extends State<EditProfileAuth2Widget> {
  late EditProfileAuth2Model _model;

  @override
  void setState(VoidCallback callback) {
    super.setState(callback);
    _model.onUpdate();
  }

  @override
  void initState() {
    super.initState();
    _model = createModel(context, () => EditProfileAuth2Model());

    _model.yourNameTextController ??=
        TextEditingController(text: currentUserDisplayName);
    _model.yourNameFocusNode ??= FocusNode();

    _model.myBioTextController ??= TextEditingController(
        text: valueOrDefault(currentUserDocument?.shortDescription, ''));
    _model.myBioFocusNode ??= FocusNode();
  }

  @override
  void dispose() {
    _model.maybeDispose();

    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return Form(
      key: _model.formKey,
      autovalidateMode: AutovalidateMode.disabled,
      child: Column(
        mainAxisSize: MainAxisSize.max,
        crossAxisAlignment: CrossAxisAlignment.start,
        children: [
          Padding(
            padding: EdgeInsetsDirectional.fromSTEB(24, 0, 0, 0),
            child: Text(
              widget!.title,
              style: FlutterFlowTheme.of(context).displaySmall.override(
                    font: GoogleFonts.interTight(
                      fontWeight:
                          FlutterFlowTheme.of(context).displaySmall.fontWeight,
                      fontStyle:
                          FlutterFlowTheme.of(context).displaySmall.fontStyle,
                    ),
                    letterSpacing: 0.0,
                    fontWeight:
                        FlutterFlowTheme.of(context).displaySmall.fontWeight,
                    fontStyle:
                        FlutterFlowTheme.of(context).displaySmall.fontStyle,
                  ),
            ),
          ),
          Padding(
            padding: EdgeInsetsDirectional.fromSTEB(24, 8, 0, 0),
            child: Text(
              'Adjust the content below to update your profile.',
              style: FlutterFlowTheme.of(context).labelLarge.override(
                    font: GoogleFonts.inter(
                      fontWeight:
                          FlutterFlowTheme.of(context).labelLarge.fontWeight,
                      fontStyle:
                          FlutterFlowTheme.of(context).labelLarge.fontStyle,
                    ),
                    letterSpacing: 0.0,
                    fontWeight:
                        FlutterFlowTheme.of(context).labelLarge.fontWeight,
                    fontStyle:
                        FlutterFlowTheme.of(context).labelLarge.fontStyle,
                  ),
            ),
          ),
          Align(
            alignment: AlignmentDirectional(0, -1),
            child: Padding(
              padding: EdgeInsetsDirectional.fromSTEB(0, 12, 0, 0),
              child: Container(
                width: 100,
                height: 100,
                decoration: BoxDecoration(
                  color: FlutterFlowTheme.of(context).accent2,
                  shape: BoxShape.circle,
                  border: Border.all(
                    color: FlutterFlowTheme.of(context).secondary,
                    width: 2,
                  ),
                ),
                child: Align(
                  alignment: AlignmentDirectional(0, 0),
                  child: Stack(
                    children: [
                      Padding(
                        padding: EdgeInsets.all(4),
                        child: AuthUserStreamWidget(
                          builder: (context) => ClipRRect(
                            borderRadius: BorderRadius.circular(60),
                            child: CachedNetworkImage(
                              fadeInDuration: Duration(milliseconds: 200),
                              fadeOutDuration: Duration(milliseconds: 200),
                              imageUrl: valueOrDefault<String>(
                                currentUserPhoto,
                                'https://images.unsplash.com/photo-1499887142886-791eca5918cd?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w0NTYyMDF8MHwxfHNlYXJjaHwxN3x8dXNlcnxlbnwwfHx8fDE2OTc4MjQ2MjZ8MA&ixlib=rb-4.0.3&q=80&w=400',
                              ),
                              width: 300,
                              height: 200,
                              fit: BoxFit.cover,
                            ),
                          ),
                        ),
                      ),
                      Padding(
                        padding: EdgeInsets.all(4),
                        child: ClipRRect(
                          borderRadius: BorderRadius.circular(60),
                          child: CachedNetworkImage(
                            fadeInDuration: Duration(milliseconds: 200),
                            fadeOutDuration: Duration(milliseconds: 200),
                            imageUrl: _model.uploadedFileUrl,
                            width: 300,
                            height: 200,
                            fit: BoxFit.cover,
                          ),
                        ),
                      ),
                    ],
                  ),
                ),
              ),
            ),
          ),
          Align(
            alignment: AlignmentDirectional(0, -1),
            child: Padding(
              padding: EdgeInsetsDirectional.fromSTEB(0, 12, 0, 32),
              child: FFButtonWidget(
                onPressed: () async {
                  final selectedMedia = await selectMedia(
                    mediaSource: MediaSource.photoGallery,
                    multiImage: false,
                  );
                  if (selectedMedia != null &&
                      selectedMedia.every(
                          (m) => validateFileFormat(m.storagePath, context))) {
                    safeSetState(() => _model.isDataUploading = true);
                    var selectedUploadedFiles = <FFUploadedFile>[];

                    var downloadUrls = <String>[];
                    try {
                      showUploadMessage(
                        context,
                        'Uploading file...',
                        showLoading: true,
                      );
                      selectedUploadedFiles = selectedMedia
                          .map((m) => FFUploadedFile(
                                name: m.storagePath.split('/').last,
                                bytes: m.bytes,
                                height: m.dimensions?.height,
                                width: m.dimensions?.width,
                                blurHash: m.blurHash,
                              ))
                          .toList();

                      downloadUrls = (await Future.wait(
                        selectedMedia.map(
                          (m) async => await uploadData(m.storagePath, m.bytes),
                        ),
                      ))
                          .where((u) => u != null)
                          .map((u) => u!)
                          .toList();
                    } finally {
                      ScaffoldMessenger.of(context).hideCurrentSnackBar();
                      _model.isDataUploading = false;
                    }
                    if (selectedUploadedFiles.length == selectedMedia.length &&
                        downloadUrls.length == selectedMedia.length) {
                      safeSetState(() {
                        _model.uploadedLocalFile = selectedUploadedFiles.first;
                        _model.uploadedFileUrl = downloadUrls.first;
                      });
                      showUploadMessage(context, 'Success!');
                    } else {
                      safeSetState(() {});
                      showUploadMessage(context, 'Failed to upload data');
                      return;
                    }
                  }
                },
                text: 'Change Photo',
                options: FFButtonOptions(
                  width: 130,
                  height: 40,
                  padding: EdgeInsetsDirectional.fromSTEB(0, 0, 0, 0),
                  iconPadding: EdgeInsetsDirectional.fromSTEB(0, 0, 0, 0),
                  color: FlutterFlowTheme.of(context).primaryBackground,
                  textStyle: FlutterFlowTheme.of(context).bodyMedium.override(
                        font: GoogleFonts.inter(
                          fontWeight: FlutterFlowTheme.of(context)
                              .bodyMedium
                              .fontWeight,
                          fontStyle:
                              FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                        ),
                        letterSpacing: 0.0,
                        fontWeight:
                            FlutterFlowTheme.of(context).bodyMedium.fontWeight,
                        fontStyle:
                            FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                      ),
                  elevation: 1,
                  borderSide: BorderSide(
                    color: FlutterFlowTheme.of(context).alternate,
                    width: 1,
                  ),
                  borderRadius: BorderRadius.circular(8),
                ),
              ),
            ),
          ),
          Padding(
            padding: EdgeInsetsDirectional.fromSTEB(20, 0, 20, 12),
            child: AuthUserStreamWidget(
              builder: (context) => TextFormField(
                controller: _model.yourNameTextController,
                focusNode: _model.yourNameFocusNode,
                autofillHints: [AutofillHints.name],
                textCapitalization: TextCapitalization.words,
                obscureText: false,
                decoration: InputDecoration(
                  labelText: 'Full Name',
                  labelStyle: FlutterFlowTheme.of(context).labelMedium.override(
                        font: GoogleFonts.inter(
                          fontWeight: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontWeight,
                          fontStyle: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontStyle,
                        ),
                        letterSpacing: 0.0,
                        fontWeight:
                            FlutterFlowTheme.of(context).labelMedium.fontWeight,
                        fontStyle:
                            FlutterFlowTheme.of(context).labelMedium.fontStyle,
                      ),
                  hintText: 'Your full name...',
                  hintStyle: FlutterFlowTheme.of(context).labelMedium.override(
                        font: GoogleFonts.inter(
                          fontWeight: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontWeight,
                          fontStyle: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontStyle,
                        ),
                        letterSpacing: 0.0,
                        fontWeight:
                            FlutterFlowTheme.of(context).labelMedium.fontWeight,
                        fontStyle:
                            FlutterFlowTheme.of(context).labelMedium.fontStyle,
                      ),
                  errorStyle: FlutterFlowTheme.of(context).bodyMedium.override(
                        font: GoogleFonts.inter(
                          fontWeight: FlutterFlowTheme.of(context)
                              .bodyMedium
                              .fontWeight,
                          fontStyle:
                              FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                        ),
                        color: FlutterFlowTheme.of(context).error,
                        letterSpacing: 0.0,
                        fontWeight:
                            FlutterFlowTheme.of(context).bodyMedium.fontWeight,
                        fontStyle:
                            FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                      ),
                  enabledBorder: OutlineInputBorder(
                    borderSide: BorderSide(
                      color: FlutterFlowTheme.of(context).alternate,
                      width: 2,
                    ),
                    borderRadius: BorderRadius.circular(8),
                  ),
                  focusedBorder: OutlineInputBorder(
                    borderSide: BorderSide(
                      color: FlutterFlowTheme.of(context).primary,
                      width: 2,
                    ),
                    borderRadius: BorderRadius.circular(8),
                  ),
                  errorBorder: OutlineInputBorder(
                    borderSide: BorderSide(
                      color: FlutterFlowTheme.of(context).error,
                      width: 2,
                    ),
                    borderRadius: BorderRadius.circular(8),
                  ),
                  focusedErrorBorder: OutlineInputBorder(
                    borderSide: BorderSide(
                      color: FlutterFlowTheme.of(context).error,
                      width: 2,
                    ),
                    borderRadius: BorderRadius.circular(8),
                  ),
                  filled: true,
                  fillColor: FlutterFlowTheme.of(context).primaryBackground,
                  contentPadding: EdgeInsetsDirectional.fromSTEB(16, 12, 0, 12),
                ),
                style: FlutterFlowTheme.of(context).bodyMedium.override(
                      font: GoogleFonts.inter(
                        fontWeight:
                            FlutterFlowTheme.of(context).bodyMedium.fontWeight,
                        fontStyle:
                            FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                      ),
                      letterSpacing: 0.0,
                      fontWeight:
                          FlutterFlowTheme.of(context).bodyMedium.fontWeight,
                      fontStyle:
                          FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                    ),
                cursorColor: FlutterFlowTheme.of(context).primary,
                validator:
                    _model.yourNameTextControllerValidator.asValidator(context),
                inputFormatters: [
                  if (!isAndroid && !isiOS)
                    TextInputFormatter.withFunction((oldValue, newValue) {
                      return TextEditingValue(
                        selection: newValue.selection,
                        text: newValue.text
                            .toCapitalization(TextCapitalization.words),
                      );
                    }),
                ],
              ),
            ),
          ),
          Padding(
            padding: EdgeInsetsDirectional.fromSTEB(20, 0, 20, 12),
            child: AuthUserStreamWidget(
              builder: (context) => FlutterFlowDropDown<String>(
                controller: _model.dropDownValueController ??=
                    FormFieldController<String>(
                  _model.dropDownValue ??=
                      valueOrDefault(currentUserDocument?.role, ''),
                ),
                options: [
                  'Owner/Founder',
                  'Director',
                  'Manager',
                  'Mid-Manager',
                  'Employee'
                ],
                onChanged: (val) =>
                    safeSetState(() => _model.dropDownValue = val),
                width: double.infinity,
                height: 44,
                textStyle: FlutterFlowTheme.of(context).bodyMedium.override(
                      font: GoogleFonts.inter(
                        fontWeight:
                            FlutterFlowTheme.of(context).bodyMedium.fontWeight,
                        fontStyle:
                            FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                      ),
                      letterSpacing: 0.0,
                      fontWeight:
                          FlutterFlowTheme.of(context).bodyMedium.fontWeight,
                      fontStyle:
                          FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                    ),
                hintText: 'Your Role',
                icon: Icon(
                  Icons.keyboard_arrow_down_rounded,
                  color: FlutterFlowTheme.of(context).secondaryText,
                  size: 24,
                ),
                fillColor: FlutterFlowTheme.of(context).primaryBackground,
                elevation: 2,
                borderColor: FlutterFlowTheme.of(context).alternate,
                borderWidth: 2,
                borderRadius: 8,
                margin: EdgeInsetsDirectional.fromSTEB(16, 4, 16, 4),
                hidesUnderline: true,
                isSearchable: false,
                isMultiSelect: false,
              ),
            ),
          ),
          Padding(
            padding: EdgeInsetsDirectional.fromSTEB(20, 0, 20, 12),
            child: AuthUserStreamWidget(
              builder: (context) => TextFormField(
                controller: _model.myBioTextController,
                focusNode: _model.myBioFocusNode,
                textCapitalization: TextCapitalization.sentences,
                obscureText: false,
                decoration: InputDecoration(
                  labelText: 'Short Description',
                  labelStyle: FlutterFlowTheme.of(context).labelMedium.override(
                        font: GoogleFonts.inter(
                          fontWeight: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontWeight,
                          fontStyle: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontStyle,
                        ),
                        letterSpacing: 0.0,
                        fontWeight:
                            FlutterFlowTheme.of(context).labelMedium.fontWeight,
                        fontStyle:
                            FlutterFlowTheme.of(context).labelMedium.fontStyle,
                      ),
                  hintText: 'A little about you...',
                  hintStyle: FlutterFlowTheme.of(context).labelMedium.override(
                        font: GoogleFonts.inter(
                          fontWeight: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontWeight,
                          fontStyle: FlutterFlowTheme.of(context)
                              .labelMedium
                              .fontStyle,
                        ),
                        letterSpacing: 0.0,
                        fontWeight:
                            FlutterFlowTheme.of(context).labelMedium.fontWeight,
                        fontStyle:
                            FlutterFlowTheme.of(context).labelMedium.fontStyle,
                      ),
                  errorStyle: FlutterFlowTheme.of(context).bodyMedium.override(
                        font: GoogleFonts.inter(
                          fontWeight: FlutterFlowTheme.of(context)
                              .bodyMedium
                              .fontWeight,
                          fontStyle:
                              FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                        ),
                        color: FlutterFlowTheme.of(context).error,
                        letterSpacing: 0.0,
                        fontWeight:
                            FlutterFlowTheme.of(context).bodyMedium.fontWeight,
                        fontStyle:
                            FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                      ),
                  enabledBorder: OutlineInputBorder(
                    borderSide: BorderSide(
                      color: FlutterFlowTheme.of(context).alternate,
                      width: 2,
                    ),
                    borderRadius: BorderRadius.circular(8),
                  ),
                  focusedBorder: OutlineInputBorder(
                    borderSide: BorderSide(
                      color: FlutterFlowTheme.of(context).primary,
                      width: 2,
                    ),
                    borderRadius: BorderRadius.circular(8),
                  ),
                  errorBorder: OutlineInputBorder(
                    borderSide: BorderSide(
                      color: FlutterFlowTheme.of(context).error,
                      width: 2,
                    ),
                    borderRadius: BorderRadius.circular(8),
                  ),
                  focusedErrorBorder: OutlineInputBorder(
                    borderSide: BorderSide(
                      color: FlutterFlowTheme.of(context).error,
                      width: 2,
                    ),
                    borderRadius: BorderRadius.circular(8),
                  ),
                  filled: true,
                  fillColor: FlutterFlowTheme.of(context).primaryBackground,
                  contentPadding: EdgeInsetsDirectional.fromSTEB(16, 12, 0, 12),
                ),
                style: FlutterFlowTheme.of(context).bodyMedium.override(
                      font: GoogleFonts.inter(
                        fontWeight:
                            FlutterFlowTheme.of(context).bodyMedium.fontWeight,
                        fontStyle:
                            FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                      ),
                      letterSpacing: 0.0,
                      fontWeight:
                          FlutterFlowTheme.of(context).bodyMedium.fontWeight,
                      fontStyle:
                          FlutterFlowTheme.of(context).bodyMedium.fontStyle,
                    ),
                textAlign: TextAlign.start,
                maxLines: 3,
                cursorColor: FlutterFlowTheme.of(context).primary,
                validator:
                    _model.myBioTextControllerValidator.asValidator(context),
                inputFormatters: [
                  if (!isAndroid && !isiOS)
                    TextInputFormatter.withFunction((oldValue, newValue) {
                      return TextEditingValue(
                        selection: newValue.selection,
                        text: newValue.text
                            .toCapitalization(TextCapitalization.sentences),
                      );
                    }),
                ],
              ),
            ),
          ),
          Align(
            alignment: AlignmentDirectional(0, 0),
            child: Padding(
              padding: EdgeInsetsDirectional.fromSTEB(20, 24, 20, 0),
              child: FFButtonWidget(
                onPressed: () async {
                  if (_model.formKey.currentState == null ||
                      !_model.formKey.currentState!.validate()) {
                    return;
                  }
                  // updateUserInfo

                  await currentUserReference!.update(createUsersRecordData(
                    displayName: _model.yourNameTextController.text,
                    photoUrl: _model.uploadedFileUrl != null &&
                            _model.uploadedFileUrl != ''
                        ? _model.uploadedFileUrl
                        : currentUserPhoto,
                    shortDescription: _model.myBioTextController.text,
                    lastActiveTime: getCurrentTimestamp,
                    role: _model.dropDownValue,
                  ));
                  ScaffoldMessenger.of(context).showSnackBar(
                    SnackBar(
                      content: Text(
                        'Profile has been updated!',
                        style: FlutterFlowTheme.of(context).titleSmall.override(
                              font: GoogleFonts.interTight(
                                fontWeight: FlutterFlowTheme.of(context)
                                    .titleSmall
                                    .fontWeight,
                                fontStyle: FlutterFlowTheme.of(context)
                                    .titleSmall
                                    .fontStyle,
                              ),
                              color: FlutterFlowTheme.of(context).info,
                              letterSpacing: 0.0,
                              fontWeight: FlutterFlowTheme.of(context)
                                  .titleSmall
                                  .fontWeight,
                              fontStyle: FlutterFlowTheme.of(context)
                                  .titleSmall
                                  .fontStyle,
                            ),
                      ),
                      duration: Duration(milliseconds: 4000),
                      backgroundColor: FlutterFlowTheme.of(context).primary,
                    ),
                  );
                  await widget.navigateAction?.call();
                },
                text: widget!.confirmButtonText,
                options: FFButtonOptions(
                  width: double.infinity,
                  height: 44,
                  padding: EdgeInsetsDirectional.fromSTEB(0, 0, 0, 0),
                  iconPadding: EdgeInsetsDirectional.fromSTEB(0, 0, 0, 0),
                  color: FlutterFlowTheme.of(context).primary,
                  textStyle: FlutterFlowTheme.of(context).titleSmall.override(
                        font: GoogleFonts.interTight(
                          fontWeight: FlutterFlowTheme.of(context)
                              .titleSmall
                              .fontWeight,
                          fontStyle:
                              FlutterFlowTheme.of(context).titleSmall.fontStyle,
                        ),
                        letterSpacing: 0.0,
                        fontWeight:
                            FlutterFlowTheme.of(context).titleSmall.fontWeight,
                        fontStyle:
                            FlutterFlowTheme.of(context).titleSmall.fontStyle,
                      ),
                  elevation: 3,
                  borderSide: BorderSide(
                    color: Colors.transparent,
                    width: 1,
                  ),
                  borderRadius: BorderRadius.circular(12),
                ),
              ),
            ),
          ),
        ],
      ),
    );
  }
}


import '/flutter_flow/flutter_flow_icon_button.dart';
import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import 'dart:ui';
import 'package:flutter/material.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:provider/provider.dart';

import 'breadcrumbs3_model.dart';
export 'breadcrumbs3_model.dart';

class Breadcrumbs3Widget extends StatefulWidget {
  const Breadcrumbs3Widget({super.key});

  @override
  State<Breadcrumbs3Widget> createState() => _Breadcrumbs3WidgetState();
}

class _Breadcrumbs3WidgetState extends State<Breadcrumbs3Widget> {
  late Breadcrumbs3Model _model;

  @override
  void setState(VoidCallback callback) {
    super.setState(callback);
    _model.onUpdate();
  }

  @override
  void initState() {
    super.initState();
    _model = createModel(context, () => Breadcrumbs3Model());
  }

  @override
  void dispose() {
    _model.maybeDispose();

    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return Padding(
      padding: EdgeInsetsDirectional.fromSTEB(0, 0, 0, 12),
      child: Container(
        width: double.infinity,
        height: 50,
        decoration: BoxDecoration(
          color: Colors.white,
          boxShadow: [
            BoxShadow(
              blurRadius: 4,
              color: Color(0x33000000),
              offset: Offset(
                0,
                2,
              ),
            )
          ],
        ),
        child: SingleChildScrollView(
          scrollDirection: Axis.horizontal,
          child: Row(
            mainAxisSize: MainAxisSize.max,
            children: [
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(15, 2, 0, 2),
                child: FlutterFlowIconButton(
                  borderColor: Colors.transparent,
                  borderRadius: 30,
                  borderWidth: 1,
                  buttonSize: 40,
                  icon: Icon(
                    Icons.home_rounded,
                    color: Color(0xFF57636C),
                    size: 22,
                  ),
                  onPressed: () {
                    print('IconButton pressed ...');
                  },
                ),
              ),
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(12, 0, 12, 0),
                child: Icon(
                  Icons.chevron_right_rounded,
                  color: Color(0xFF57636C),
                  size: 16,
                ),
              ),
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(0, 8, 0, 8),
                child: Container(
                  decoration: BoxDecoration(
                    color: Colors.white,
                  ),
                  alignment: AlignmentDirectional(0, 0),
                  child: Padding(
                    padding: EdgeInsetsDirectional.fromSTEB(16, 0, 16, 0),
                    child: Text(
                      'Page Title',
                      style: FlutterFlowTheme.of(context).labelLarge.override(
                            font: GoogleFonts.readexPro(
                              fontWeight: FontWeight.normal,
                              fontStyle: FlutterFlowTheme.of(context)
                                  .labelLarge
                                  .fontStyle,
                            ),
                            color: Color(0xFF57636C),
                            fontSize: 16,
                            letterSpacing: 0.0,
                            fontWeight: FontWeight.normal,
                            fontStyle: FlutterFlowTheme.of(context)
                                .labelLarge
                                .fontStyle,
                          ),
                    ),
                  ),
                ),
              ),
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(12, 0, 12, 0),
                child: Icon(
                  Icons.chevron_right_rounded,
                  color: Color(0xFF57636C),
                  size: 16,
                ),
              ),
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(0, 8, 16, 8),
                child: Container(
                  decoration: BoxDecoration(
                    color: Color(0xFFF1F4F8),
                    borderRadius: BorderRadius.circular(8),
                  ),
                  alignment: AlignmentDirectional(0, 0),
                  child: Padding(
                    padding: EdgeInsetsDirectional.fromSTEB(16, 0, 16, 0),
                    child: Text(
                      'Page Details',
                      style: FlutterFlowTheme.of(context).bodyLarge.override(
                            font: GoogleFonts.readexPro(
                              fontWeight: FontWeight.normal,
                              fontStyle: FlutterFlowTheme.of(context)
                                  .bodyLarge
                                  .fontStyle,
                            ),
                            color: Color(0xFF14181B),
                            fontSize: 16,
                            letterSpacing: 0.0,
                            fontWeight: FontWeight.normal,
                            fontStyle: FlutterFlowTheme.of(context)
                                .bodyLarge
                                .fontStyle,
                          ),
                    ),
                  ),
                ),
              ),
            ],
          ),
        ),
      ),
    );
  }
}


import '/flutter_flow/flutter_flow_icon_button.dart';
import '/flutter_flow/flutter_flow_theme.dart';
import '/flutter_flow/flutter_flow_util.dart';
import 'dart:ui';
import 'package:flutter/material.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:provider/provider.dart';

import 'breadcrumbs_model.dart';
export 'breadcrumbs_model.dart';

class BreadcrumbsWidget extends StatefulWidget {
  const BreadcrumbsWidget({super.key});

  @override
  State<BreadcrumbsWidget> createState() => _BreadcrumbsWidgetState();
}

class _BreadcrumbsWidgetState extends State<BreadcrumbsWidget> {
  late BreadcrumbsModel _model;

  @override
  void setState(VoidCallback callback) {
    super.setState(callback);
    _model.onUpdate();
  }

  @override
  void initState() {
    super.initState();
    _model = createModel(context, () => BreadcrumbsModel());
  }

  @override
  void dispose() {
    _model.maybeDispose();

    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return Padding(
      padding: EdgeInsetsDirectional.fromSTEB(0, 0, 0, 12),
      child: Container(
        width: double.infinity,
        height: 50,
        decoration: BoxDecoration(
          color: Colors.white,
          boxShadow: [
            BoxShadow(
              blurRadius: 4,
              color: Color(0x33000000),
              offset: Offset(
                0,
                2,
              ),
            )
          ],
        ),
        child: SingleChildScrollView(
          scrollDirection: Axis.horizontal,
          child: Row(
            mainAxisSize: MainAxisSize.max,
            children: [
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(15, 2, 0, 2),
                child: FlutterFlowIconButton(
                  borderColor: Colors.transparent,
                  borderRadius: 30,
                  borderWidth: 1,
                  buttonSize: 40,
                  icon: Icon(
                    Icons.home_rounded,
                    color: Color(0xFF57636C),
                    size: 22,
                  ),
                  onPressed: () {
                    print('IconButton pressed ...');
                  },
                ),
              ),
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(12, 0, 12, 0),
                child: Icon(
                  Icons.chevron_right_rounded,
                  color: Color(0xFF57636C),
                  size: 16,
                ),
              ),
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(0, 8, 0, 8),
                child: Container(
                  decoration: BoxDecoration(
                    color: Colors.white,
                  ),
                  alignment: AlignmentDirectional(0, 0),
                  child: Padding(
                    padding: EdgeInsetsDirectional.fromSTEB(16, 0, 16, 0),
                    child: Text(
                      'Page Title',
                      style: FlutterFlowTheme.of(context).labelLarge.override(
                            font: GoogleFonts.readexPro(
                              fontWeight: FontWeight.normal,
                              fontStyle: FlutterFlowTheme.of(context)
                                  .labelLarge
                                  .fontStyle,
                            ),
                            color: Color(0xFF57636C),
                            fontSize: 16,
                            letterSpacing: 0.0,
                            fontWeight: FontWeight.normal,
                            fontStyle: FlutterFlowTheme.of(context)
                                .labelLarge
                                .fontStyle,
                          ),
                    ),
                  ),
                ),
              ),
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(12, 0, 12, 0),
                child: Icon(
                  Icons.chevron_right_rounded,
                  color: Color(0xFF57636C),
                  size: 16,
                ),
              ),
              Padding(
                padding: EdgeInsetsDirectional.fromSTEB(0, 8, 16, 8),
                child: Container(
                  decoration: BoxDecoration(
                    color: Color(0xFFF1F4F8),
                    borderRadius: BorderRadius.circular(8),
                  ),
                  alignment: AlignmentDirectional(0, 0),
                  child: Padding(
                    padding: EdgeInsetsDirectional.fromSTEB(16, 0, 16, 0),
                    child: Text(
                      'Page Details',
                      style: FlutterFlowTheme.of(context).bodyLarge.override(
                            font: GoogleFonts.readexPro(
                              fontWeight: FontWeight.normal,
                              fontStyle: FlutterFlowTheme.of(context)
                                  .bodyLarge
                                  .fontStyle,
                            ),
                            color: Color(0xFF14181B),
                            fontSize: 16,
                            letterSpacing: 0.0,
                            fontWeight: FontWeight.normal,
                            fontStyle: FlutterFlowTheme.of(context)
                                .bodyLarge
                                .fontStyle,
                          ),
                    ),
                  ),
                ),
              ),
            ],
          ),
        ),
      ),
    );
  }
}


import 'dart:convert';
import 'dart:math' as math;

import 'package:flutter/material.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:intl/intl.dart';
import 'package:timeago/timeago.dart' as timeago;
import 'lat_lng.dart';
import 'place.dart';
import 'uploaded_file.dart';
import '/backend/backend.dart';
import 'package:cloud_firestore/cloud_firestore.dart';
import '/auth/firebase_auth/auth_util.dart';

double? priceSummary(List<double>? prices) {
// summarize a list of prices from the product list
  if (prices == null || prices.isEmpty) {
    return null;
  }
  return prices.reduce((value, element) => value + element);
}


name: hospedagem_simples
description: A new Flutter project.

environment:
  sdk: ">=3.0.0 <4.0.0"

dependencies:
  flutter:
    sdk: flutter
  auto_size_text: 3.0.0
  badges: 2.0.2
  cached_network_image: 3.4.1
  cached_network_image_platform_interface: 4.1.1
  cached_network_image_web: 1.3.1
  cloud_firestore: 5.5.0
  cloud_firestore_platform_interface: 6.5.0
  cloud_firestore_web: 4.3.4
  collection: 1.19.0
  csslib: 0.17.3
  dropdown_button2: 2.3.9
  easy_debounce: 2.0.1
  file_picker: 8.1.2
  firebase_auth: 5.3.3
  firebase_auth_platform_interface: 7.4.9
  firebase_auth_web: 5.13.4
  firebase_core: 3.8.0
  firebase_core_platform_interface: 5.3.0
  firebase_core_web: 2.18.1
  flutter_animate: 4.5.0
  flutter_cache_manager: 3.4.1
  flutter_plugin_android_lifecycle: 2.0.20
  flutter_rating_bar: 4.0.1
  font_awesome_flutter: 10.7.0
  from_css_color: 2.0.0
  go_router: 12.1.3
  google_fonts: 6.1.0
  google_sign_in: 6.2.1
  google_sign_in_android: 6.1.30
  google_sign_in_ios: 5.7.7
  google_sign_in_platform_interface: 2.4.5
  google_sign_in_web: 0.12.4+2
  html: 0.15.4
  image_picker: 1.1.2
  image_picker_android: 0.8.12+13
  image_picker_for_web: 3.0.5
  image_picker_ios: 0.8.12
  image_picker_linux: 0.2.1+1
  image_picker_macos: 0.2.1+1
  image_picker_platform_interface: 2.10.0
  image_picker_windows: 0.2.1+1
  intl: 0.19.0
  json_path: 0.7.2
  mask_text_input_formatter: 2.9.0
  mime_type: 1.0.0
  page_transition: 2.1.0
  path_provider: 2.1.4
  path_provider_android: 2.2.10
  path_provider_foundation: 2.4.0
  path_provider_linux: 2.2.1
  path_provider_platform_interface: 2.1.2
  path_provider_windows: 2.3.0
  plugin_platform_interface: 2.1.8
  provider: 6.1.2
  rxdart: 0.27.7
  shared_preferences: 2.3.2
  shared_preferences_android: 2.3.2
  shared_preferences_foundation: 2.5.2
  shared_preferences_linux: 2.4.1
  shared_preferences_platform_interface: 2.4.1
  shared_preferences_web: 2.4.2
  shared_preferences_windows: 2.4.1
  sign_in_with_apple: 6.1.2
  sign_in_with_apple_platform_interface: 1.1.0
  sign_in_with_apple_web: 2.1.0
  smooth_page_indicator: 1.1.0
  sqflite: 2.3.3+1
  sqflite_common: 2.5.4+3
  stream_transform: 2.1.0
  timeago: 3.6.1
  url_launcher: 6.3.0
  url_launcher_android: 6.3.10
  url_launcher_ios: 6.3.1
  url_launcher_linux: 3.2.0
  url_launcher_macos: 3.2.1
  url_launcher_platform_interface: 2.3.2
  url_launcher_web: 2.3.3
  url_launcher_windows: 3.1.2
  video_player: 2.9.2
  video_player_android: 2.7.13
  video_player_avfoundation: 2.6.2
  video_player_platform_interface: 6.2.3
  video_player_web: 2.3.2

dev_dependencies:
  flutter_lints: 4.0.0
  lints: 4.0.0
  flutter_test:
    sdk: flutter

flutter:
  uses-material-design: true
  assets:
    - assets/images/
    - assets/videos/
    - assets/audios/
    - assets/rive_animations/
    - assets/pdfs/
    - assets/jsons/


  rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /users/{document} {
      allow create: if true;
      allow read: if true;
      allow write: if true;
      allow delete: if true;
    }

    match /products/{document} {
      allow create: if true;
      allow read: if true;
      allow write: if true;
      allow delete: if true;
    }

    match /orders/{document} {
      allow create: if true;
      allow read: if true;
      allow write: if true;
      allow delete: if true;
    }

    match /RoomType/{document} {
      allow create: if true;
      allow read: if true;
      allow write: if true;
      allow delete: if true;
    }
  }
}


{
  "indexes": [
    {
      "collectionGroup": "orders",
      "queryScope": "COLLECTION",
      "fields": [
        {
          "fieldPath": "owner",
          "order": "ASCENDING"
        },
        {
          "fieldPath": "timeCreated",
          "order": "DESCENDING"
        }
      ]
    }
  ]
}
