## COCOLANG 

#### Getting COCO version
```
coco version
```

#### Initiating COCO (generate coco.nut file)
```
coco nut init <app-name>
```

#### Compiling COCO
```
coco compile
```

#### Format of Project
<ol>
    <li>Module Name</li>
    <li> Persistent State - (think of it as a db)</li>
        <ol>
            <li>variables</li>
        </ol>
    <li>Endpoints - (think of it as API's)</li>
        <ol>
            <li>deployer - (called only while deploying logic)</li>
            <li>invokable - </li>
                <ol>
                    <li>non-mutating / read endpoints - (only to read from the logic)</li>
                    <li>mutating - (will change the peristent state of the logic) - "!" after the name of the endpoint</li>
                </ol>
        </ol>
    <li>func - internal functions (can only be called inside the logic)</li>
</ol>
