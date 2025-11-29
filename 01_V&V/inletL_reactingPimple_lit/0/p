/*--------------------------------*- C++ -*----------------------------------*\
| =========                 |                                                 |
| \\      /  F ield         | OpenFOAM: The Open Source CFD Toolbox           |
|  \\    /   O peration     | Version:  v2012                                 |
|   \\  /    A nd           | Website:  www.openfoam.com                      |
|    \\/     M anipulation  |                                                 |
\*---------------------------------------------------------------------------*/
FoamFile
{
    version     2.0;
    format      ascii;
    class       volScalarField;
    object      p;
}
// * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * //

dimensions      [1 -1 -2 0 0 0 0];

// 1.22 kPa = 1220 Pa
internalField   uniform 1220;

boundaryField
{
    P.Inlet
    {
        type        fixedValue;
        value       uniform 1220;
    }

    P.Outlet
    {
        // For supersonic exit, zeroGradient is standard for p
        type        zeroGradient;
    }

    Farfield
    {
        type        zeroGradient;
    }

    Wall
    {
        type        zeroGradient;
    }

    Symmetry
    {
        type        symmetryPlane;
    }

    patch0
    {
        type        empty;
    }

    patch3
    {
        type        empty;
    }
}