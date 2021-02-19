<html xmlns="http://www.w3.org/TR/xhtml1/strict">
  <head>
  </head>
  <body>
    <h1>Business Object Definition</h1>
    <h2>About this document...</h2>
    <div>The Business Object Definition describes the APIs available within a single business object, their parameters and their behaviours from both a business and technical perspective. The definition of each object function describes the business function of the interface, the parameters and usage of the business function and any technical notes required in the on-going support of the interface, including reference to the capabilities of the object. The Business Object Definition API is a dual-purpose document designed to serve the needs of both business users and technical system support staff who require information relating to the business functions available and their details. As such, the BOD is a working document and is subject to change during the course of development and implementation.</div>
    <h2>About Business Objects</h2>
    <div>Business Objects within the environment (i.e. objects which may be drawn onto a process to capture and replicate a part of a business process) adhere to strict guidelines in their implementation. The definition and behaviour of the object both as seen in Process Studio during design time and as implemented during test or via Control Room at runtime uses the same interface definition, known as an object's capabilities. All business objects used within Blue Prism, generic and bespoke, have a common property - Get Capabilities. The GetCapabilities function returns an XML formatted string which defines the interfaces for that object, their friendly names (as they appear in Process Studio) and any inputs and outputs that are required. The Business Object Definition object captures the name, parameters, preconditions and endpoints of each function relating to a business object and translates to the object definition seen within Process Studio.</div>
    <h2>1.0 Data - OLEDB</h2>
    <div>A SQL interface for interacting with OLEDB data sources</div>
    <p>The runmode of this business object is "background"</p>
    <h3>1.1 Close</h3>
    <div>Closes the connection to the OLEDB database.</div>
    <h3>1.2 Execute</h3>
    <div />
    <table>
      <tr>
        <th>Parameter</th>
        <th>Direction</th>
        <th>Data Type</th>
        <th>Description</th>
      </tr>
      <tr>
        <td>SQL</td>
        <td>In</td>
        <td>Text</td>
        <td />
      </tr>
    </table>
    <h3>1.3 Get Collection</h3>
    <div />
    <table>
      <tr>
        <th>Parameter</th>
        <th>Direction</th>
        <th>Data Type</th>
        <th>Description</th>
      </tr>
      <tr>
        <td>SQL</td>
        <td>In</td>
        <td>Text</td>
        <td>An SQL query to fetch the data. In most cases this will be a 'select' query.</td>
      </tr>
      <tr>
        <td>Results</td>
        <td>Out</td>
        <td>Collection</td>
        <td />
      </tr>
    </table>
    <h3>1.4 Open</h3>
    <div>Opens a connection to the OLEDB database.</div>
    <h3>1.5 Set Connection</h3>
    <div>Sets the connection details for the database.</div>
    <h4>Preconditions:</h4>
    <div />
    <table>
      <tr>
        <th>Parameter</th>
        <th>Direction</th>
        <th>Data Type</th>
        <th>Description</th>
      </tr>
      <tr>
        <td>Database</td>
        <td>In</td>
        <td>Text</td>
        <td>Optional. The path to the oledb database file</td>
      </tr>
      <tr>
        <td>Password</td>
        <td>In</td>
        <td>Password</td>
        <td>Optional. The password if required to open the oledb database.</td>
      </tr>
      <tr>
        <td>Provider</td>
        <td>In</td>
        <td>Text</td>
        <td>Optional. Allows the database provider to be overridden.</td>
      </tr>
      <tr>
        <td>Connection String</td>
        <td>In</td>
        <td>Text</td>
        <td>Optional. Allows the full connection string to be provided. If supplying this parameter no other parameters are required.</td>
      </tr>
    </table>
  </body>
</html>
