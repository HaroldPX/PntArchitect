# Controller Manager :id=controllermanager

The content manager is a method that allows you to use parameters from the simulation without defining them in the parameter controller. Below is an example of the syntax for using the content manager.

"// Controller Code

CO_Object tapis; //Pointeur vers le tapis

CO_Object cell; //Pointeur vers la cellule

public void _Init()
{
    // Get the list of products in the scene

    int count = ContentManager.Products.Count;

    //initialisation du pointeur pars l'ID de l'objet 
    tapis = ContentManager.GetObjectById(9);
    //initialisation du pointeur pars le nom de l'objet 
    cell = ContentManager.GetObjectByName("C101");
    SendMessage("Log", "Object Name " + tapis.Name);

    // Access the Disjoncteur object from the carpet object
    CO_Object disj = tapis.Parent.Child["Disjoncteur"];
}

public void _Loop()
{
   // Read the value of the cell using an enum
    bool val = (bool)cell.Data[EAttributs.DI_Valeur];
    // Write the value of the motor command using an ID
    tapis.Data[5] = !val;

    // Read the value of the "Marche" button (button name)
    bool val2 = (bool)tapis.Button["Marche"];
    // Write the value of button 1
    tapis.Button[1] = val2;

    // Read a CAB on a cell.
    if (val && cell.Colliders.Count > 0)
    {
        string V_CAB = ContentManager.GetProductById(cell.Colliders[0]).Property["CAB"];
    }
}"

<table>
        <tbody><tr>
            <th>Function</th>
            <th>Description</th>
            <th>Input/Output</th>
        </tr>
        <tr>
            <td>ContentManager.GetProductById</td>
            <td>Read A CAB on a cell.</td>
            <td>Cell/CAB.</td>
        </tr>
</tbody></table>

