Installing #SNMP Library on Windows
===================================

By `Lex Li`_

This page shows you how to install #SNMP Library to your project on Windows. 

.. contents:: In this article:
  :local:
  :depth: 1

Install #SNMP Library via NuGet
-------------------------------

The easiest way to get started building applications with #SNMP Library is to install via NuGet in the latest version of Visual Studio 2015 (including the free Community edition). 

1. Install `Visual Studio 2015 <https://go.microsoft.com/fwlink/?LinkId=532606>`_.

  Be sure to specify that you include the Windows and Web Development.

2. Install latest `NuGet Package Manager <https://docs.nuget.org/consume/installing-nuget>`_. 

  This will install the latest NuGet tooling.

3. Open/create an empty Windows Forms project.
  
4. Install #SNMP Library NuGet packages following `NuGet conventions <https://docs.nuget.org/Consume/Package-Manager-Dialog>`_. 

  The latest package can be found at,

  * `Main Library <https://www.nuget.org/packages/Lextm.SharpSnmpLib/>`_. 
  * `Platform Extensions <https://www.nuget.org/packages/Lextm.SharpSnmpLib.Extensions/>`_ (Required by release 10.0.0 only. Not required any more for 10.0.1 and above.)

.. note:: In 10.0.0 release, the platform extensions package is required for .NET Framework, Xamarin.iOS, and Xamarin.Android applications so as to use DES/AES encryption. This package is no longer
   needed in release 10.0.1 and above.

Install #SNMP Library via source code
-------------------------------------

#SNMP Library source code can be directly used in your project. 

1. Download the source code from `GitHub <https://github.com/lextm/sharpsnmplib/releases>`_, or clone the repo directly.

2. Run ``prepare.bat`` on Windows (or ``prepare.sh`` on non-Windows platforms) to prepare the code base for compilation.

3. Open/create a empty Windows Forms project in a solution.

4. Add SharpSnmpLib.csproj (release 10.0 and above), and SharpSnmpLib.Full.csproj (10.0.0) in ``SharpSnmpLib`` directory to your solution.

.. note:: SharpSnmpLib.Android.csproj and SharpSnmpLib.iOS.csproj might be used to target Xamarin platforms for release 10.0.0. They are no longer needed for 10.0.1 release and above.

Related Resources
-----------------

- :doc:`/tutorials/introduction`
- :doc:`/tutorials/v3-operations`
- :doc:`/samples/command-line-tools`
- :doc:`/samples/agent-development`
