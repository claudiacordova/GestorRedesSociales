# GestorRedesSociales

<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml"
      xmlns:ui="http://java.sun.com/jsf/facelets"
      xmlns:h="http://java.sun.com/jsf/html"
      xmlns:f="http://java.sun.com/jsf/core"
      xmlns:p="http://primefaces.org/ui">

    <ui:composition template="/WEB-INF/include/template.xhtml">
        <ui:define name="title">
            <h:outputText value="#{myBundle.AppName}"></h:outputText>
        </ui:define>
        <ui:define name="body">
            <p:panel header="PLATAFORMA">
                <p> <h:outputLabel rendered="#{templateController.esAdmin()}" value="   Bienvenido Administrador!  " />
            <h:outputLabel rendered="#{!templateController.esAdmin()}" value="   Bienvenido Usuario!  " />
            </p>
            </p:panel>

        </ui:define>

    </ui:composition>

</html>
