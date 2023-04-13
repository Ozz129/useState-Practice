import React,{ useEffect, useState } from "react";

function Saludar() {

    const [estudiantes, setEstudiantes] = useState(0);
    const [estudiantes2, setEstudiantes2] = useState(0);

    function incrementar() {
        setEstudiantes(estudiantes + 1);
    }

    /**
     * useEffect => function que recibe
     *  callback => Es una función que se pasa como parametro a otra función
     *              Es la función que se va a ejecutar, cuando se ejecute el hook
     *  dependencias => Son valoes que van a desencadenar la ejecución del calback
     */
    useEffect(() => {
        /**
         * Indicaciones que se van a cumplir cuando el valor de las dependencias cambie
         */
        alert('Hola muchachos')
        
    }, [])

    return(
        <div>
            <button onClick={incrementar}>Ingresar a la sesión</button>
        </div>
    )
}
export default Saludar;
